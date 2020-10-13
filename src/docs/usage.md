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
* execute `./igpop.sh dev` in the command line to run a local server on 8899 (may be changed with `-p` param)
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

## Publish the Implementation Guide
---

- Download the [FHIR publisher tool](https://github.com/HL7/fhir-ig-publisher/releases). The FHIR documentation can be found [here](https://confluence.hl7.org/display/FHIR/IG+Publisher+Documentation#IGPublisherDocumentation-Installing)
- Access the ig-ae/ig folder. The folder contains the `ig.ini` file and the `input` folder
- Run the publisher in the GUI mode by double clicking the `publisher.jar` file, or run it in the console with the following command:<br>
`java -jar publisher.jar -ig ig.ini`
- After the process is finished, access the `output` folder and open `index.html` file - this will be the home page of the published IG.



