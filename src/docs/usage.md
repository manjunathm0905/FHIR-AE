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

## Validate Generated Structure Definitions
--- 

```java -jar validator_cli.jar -version 4.0.1 adverse-event-profile34/* -ig adverse-event-profile34/ -recurse```



