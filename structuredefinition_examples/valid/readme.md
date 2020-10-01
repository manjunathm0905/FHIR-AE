AZAdverseEvent.json - valid StructureDefinition AdverseEvent profile - this is an example of what igpop should generate for resource profiles
AZEmployeeReporter.json - valid StructureDefinition of AZEmployeeReporter extension - this is an example of what igpop should generate for extensions
original-\*.json - sample FHIR StructureDefinition files

To run FHIR validator:

$ java -jar validator_cli.jar -version 4.0.1 AZAdverseEvent.json -no-extensible-binding-warnings
$ java -jar validator_cli.jar -version 4.0.1 AZEmployeeReporter.json -no-extensible-binding-warnings


Also, we will need to set correct urls in our generated StructureDefinitions
to resolve these warnings:
  Warning @ StructureDefinition.differential.element.where(path = 'AdverseEvent.extension:AZEmployeeReporter') : The type of profile https://healthsamurai.github.io/ig-ae/profiles/StructureDefinition/AZEmployeeReporter cannot be checked as the profile is not known
