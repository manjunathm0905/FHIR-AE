---
title: Instruction
---

# Instruction
---
---

## Generate Structure Definitions
---

- Click the Package link to generate a package of FHIR StructureDefinitions and ValueSets
- The package will be downloaded as a zip-archive
- Unzip the archive
- Browse the folder
- The folder will contain FHIR StructureDefinitions and ValueSets

## Run IGPOP Locally
---

- Clone the repository [https://github.com/HealthSamurai/ig-ae](https://github.com/HealthSamurai/ig-ae)
- Access the repository folder
- Run the command: `java -jar "./igpop/target/igpop.jar" dev -p 8891`
- Open localhost:8891


## Publish the Implementation Guide
---

- Download the [FHIR publisher tool](https://github.com/HL7/fhir-ig-publisher/releases). The FHIR documentation can be found [here](https://confluence.hl7.org/display/FHIR/IG+Publisher+Documentation#IGPublisherDocumentation-Installing)
- Access the ig-ae/ig folder. The folder contains the `ig.ini` file and the `input` folder
- Run the publisher in the GUI mode by double clicking the `publisher.jar` file, or run it in the console with the following command:<br>
`java -jar publisher.jar -ig ig.ini`
- After the process is finished, access the `output` folder and open `index.html` file - this will be the home page of the published IG.



