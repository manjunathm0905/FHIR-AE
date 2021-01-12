---
title: Instructions
---

# Instructions
---
---

## Development
---

### Run a Local Server
---

In order to develop the implementation guide, do the following steps:

- Clone the repository [https://github.com/HealthSamurai/ig-ae](https://github.com/HealthSamurai/ig-ae)

```git clone https://github.com/HealthSamurai/ig-ae.git```

- browse to the ig-ae folder

```cd ig-ae```

- Install modules

```npm install```

- Init submodules

```git submodule init```

- Update submodules

```git submodule update```

- Run a local server on the 8891 port (or specify another port if needed)

```./igpop.sh dev -p 8891```

- Navigate to the [http://localhost:8891](http://localhost:8891) to see results of editing

Console output:

```/ig-ae
$ ./igpop.sh dev -p 8891
Dev... (dev -p 8891)
Run server on http://localhost: 8891
```


### Project Structure and Configuration
---

![Project structure](https://github.com/HealthSamurai/ig-ae/blob/master/src/images/project_structure.png?raw=true)


- Update the ig.yaml file in the project root folder:

`id:`  prefix for your FHIR resources<br>
`title:` title displayed on the home page of your IG site<br>
`url:` base URL for your profiles (StructureDefinition.url and fixedUri)<br>
`description:` your IG general description<br>
`fhir:` FHIR version (current value is 4.0.0)<br>


![ig.yaml](https://github.com/HealthSamurai/ig-ae/blob/master/src/images/igyaml.png?raw=true)

- You will need to stop and start server to apply ig.yaml changes


## Edit Profiles and ValueSets
---

When you are running profiles locally, you can edit them directly on the site:

![Editing](https://github.com/HealthSamurai/ig-ae/blob/master/src/images/editing.gif?raw=true)


## Generate Structure Definitions
---

- Click the Package link to generate a package of FHIR StructureDefinitions and ValueSets
- The package will be downloaded as a zip-archive
- Unzip the archive
- Browse the folder
- The folder will contain FHIR StructureDefinitions and ValueSets

![Package](https://github.com/HealthSamurai/ig-ae/blob/master/src/images/package.gif?raw=true)

## Validate Generated Structure Definitions
--- 

- Having that you downloaded and unzipped the archive with generated structure definitions, you can validate them against the base FHIR specification and your IG.
- Download the official FHIR [validator](https://github.com/hapifhir/org.hl7.fhir.core/releases/latest/download/validator_cli.jar) — a Java jar file that can be used to validate resources ([download page](http://build.fhir.org/downloads.html)). (See the [Validator documentation](https://confluence.hl7.org/display/FHIR/Using+the+FHIR+Validator))
- Say, you've extracted files to the `adverse-event-profile` folder. Then, you will run the following command from the parent folder.
- Remove the package.json file from the `adverse-event-profile` folder
- Run the validator:

```java -jar validator_cli.jar -version 4.0.1 adverse-event-profile/* -ig adverse-event-profile/ -recurse```

See more [Using the FHIR Validator](https://confluence.hl7.org/display/FHIR/Using+the+FHIR+Validator).


## Validate Resources against Profiles
--- 

### Validate against a profile

- You can specify profile to validate against in the command:

```java -jar validator_cli.jar -version 4.0.1 path/to/resource -ig path/to/ig/folder/ -recurse -profile profile/StructureDefinition/url```

- Example:

```java -jar validator_cli.jar -version 4.0.1 resourcesToValidate/adverseEventSample.json -ig adverse-event-profile/ -recurse -profile https://semalexa.github.io/ig-az/StructureDefinition/hl7.fhir.ae-AdverseEvent```

### Validate a resource

- You can specify profiles to validate against in the resource:
```
"meta": {
    "profile": ["https://semalexa.github.io/ig-az/StructureDefinition/hl7.fhir.ae-AdverseEvent"]
  }
```  
  
- Then, you can run the following command:  

```java -jar validator_cli.jar -version 4.0.1 path/to/resource -ig path/to/ig/folder/ -recurse```

- Example:
  
```java -jar validator_cli.jar -version 4.0.1 resourcesToValidate/adverseEventSample.json -ig adverse-event-profile/ -recurse```

### Validate against a FHIR Package

[Sample FHIR Package](http://registry.fhir.org/package/hl7.fhir.us.patient-reported-outcomes%7C0.2.0)

```java -jar validator_cli.jar -version 4.0.1 resourcesToValidate/adverseEventSample.json -ig hl7.fhir.us.patient-reported-outcomes```

### Validate against a profile by URL


```java -jar validator_cli.jar -version 4.0.1 resourcesToValidate/adverseEventSample.json -ig https://healthsamurai.github.io/ig-ae/StructureDefinition/hl7.fhir.ae-AdverseEvent.json  -profile https://semalexa.github.io/ig-az/StructureDefinition/hl7.fhir.ae-AdverseEvent```

In the future, it could work this way:

```java -jar validator_cli.jar -version 4.0.1 resourcesToValidate/adverseEventSample.json -ig https://healthsamurai.github.io/ig-ae/StructureDefinition/hl7.fhir.ae-AdverseEvent.json -ig https://healthsamurai.github.io/ig-ae/StructureDefinition/hl7.fhir.ae-AdverseEvent-AZEmployeeReporter.json -ig https://healthsamurai.github.io/ig-ae/StructureDefinition/hl7.fhir.ae-AdverseEvent-lateReason.json -ig https://healthsamurai.github.io/ig-ae/StructureDefinition/hl7.fhir.ae-AdverseEvent-localReference.json -ig https://healthsamurai.github.io/ig-ae/StructureDefinition/hl7.fhir.ae-AdverseEvent-positiveDechallenge.json -ig https://healthsamurai.github.io/ig-ae/StructureDefinition/hl7.fhir.ae-AdverseEvent-positiveRechallenge.json -ig https://healthsamurai.github.io/ig-ae/StructureDefinition/hl7.fhir.ae-AdverseEvent-programNumber.json -ig https://healthsamurai.github.io/ig-ae/StructureDefinition/hl7.fhir.ae-AdverseEvent-rechallenge.json -ig https://healthsamurai.github.io/ig-ae/StructureDefinition/hl7.fhir.ae-AdverseEvent-reporterType.json -ig https://healthsamurai.github.io/ig-ae/StructureDefinition/hl7.fhir.ae-AdverseEvent-sourceType.json -ig https://healthsamurai.github.io/ig-ae/StructureDefinition/hl7.fhir.ae-AdverseEvent-surveyStatus.json -ig https://healthsamurai.github.io/ig-ae/ValueSet/hl7.fhir.ae-survey-status.json -ig https://healthsamurai.github.io/ig-ae/ValueSet/hl7.fhir.ae-intelligent-source.json```

## Create new profile

See the [IGPOP spec](https://github.com/HealthSamurai/igpop/blob/master/igpop.md).

