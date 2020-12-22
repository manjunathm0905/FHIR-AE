---
title: Instructions
---

# Instructions
---
---

## Development
---

In order to develop the implementation guide, do the following steps:

* clone the repository [https://github.com/HealthSamurai/ig-ae](https://github.com/HealthSamurai/ig-ae)
* execute `npm install` in a command line
* execute `./igpop.sh dev` in the command line to run a local server on 8899 by default (may be changed with `-p` param e.g. `./igpop.sh dev -p 8799`)
* navigate to `http://localhost:8899` to see results of editing



## Alternative Development (with igpop.jar file)

- Clone the repository
- Access the repository folder
- Run the command: `java -jar "./igpop/target/igpop.jar" dev -p 8891`
- Open localhost:8891

## Generate Structure Definitions
---

- Click the Package link to generate a package of FHIR StructureDefinitions and ValueSets
- The package will be downloaded as a zip-archive
- Unzip the archive
- Browse the folder
- The folder will contain FHIR StructureDefinitions and ValueSets

## Validate Generated Structure Definitions
--- 

- Having that you downloaded and unzipped the archive with generated structure definitions, you can validate them against the base FHIR specification and your IG.
- Download the official FHIR validator - a Java jar file that can be used to validate resources (http://build.fhir.org/downloads.html).
- Say you've extracted files to the adverse-event-profile folder. Then you will run the following command:

```java -jar validator_cli.jar -version 4.0.1 adverse-event-profile/* -ig adverse-event-profile/ -recurse```


## Validate your custom resources
--- 