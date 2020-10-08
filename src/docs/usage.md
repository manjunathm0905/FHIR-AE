---
title: Instruction
---

# Instruction

Clone the repository

Access the repository folder

Run the command:

```
java -jar "./igpop/target/igpop.jar" dev -p 8891
```

Open localhost:8891

Click the Package link to generate a package of FHIR StructureDefinitions and ValueSets

The package will be downloaded as a zip-archive

Unzip the archive

Browse the folder

The folder will contain FHIR StractureDefinitions and ValueSets

## StractureDefinitions


**File**|**Description**|**Status**|**FHIR Validator Output**
-----|-----|-----|-----
hl7.fhir.ae-Address.json| |`Invalid` | *FAILURE*: 5 errors, 2 warnings, 0 notes
hl7.fhir.ae-Address-region.json| |`Invalid` |*FAILURE*: 1 errors, 1 warnings, 0 notes 
hl7.fhir.ae-AdverseEvent.json| | Valid | Success: 0 errors, 10 warnings, 0 notes
hl7.fhir.ae-AdverseEvent-AZEmployeeReporter.json| |`Invalid` | *FAILURE*: 1 errors, 0 warnings, 0 notes
hl7.fhir.ae-AdverseEvent-lateReason.json| |`Invalid` | *FAILURE*: 1 errors, 1 warnings, 0 notes
hl7.fhir.ae-AdverseEvent-localReference.json| | `Invalid`| *FAILURE*: 1 errors, 1 warnings, 0 notes
hl7.fhir.ae-AdverseEvent-positiveDechallenge.json| | `Invalid`| *FAILURE*: 1 errors, 1 warnings, 0 notes
hl7.fhir.ae-AdverseEvent-positiveRechallenge.json| | `Invalid`| *FAILURE*: 1 errors, 1 warnings, 0 notes
hl7.fhir.ae-AdverseEvent-programNumber.json| |`Invalid` | *FAILURE*: 1 errors, 1 warnings, 0 notes
hl7.fhir.ae-AdverseEvent-rechallenge.json| |`Invalid` | *FAILURE*: 1 errors, 1 warnings, 0 notes
hl7.fhir.ae-AdverseEvent-reporterType.json| |`Invalid` |*FAILURE*: 1 errors, 1 warnings, 0 notes 
hl7.fhir.ae-AdverseEvent-sourceType.json| | `Invalid`| *FAILURE*: 1 errors, 1 warnings, 0 notes
hl7.fhir.ae-AdverseEvent-surveyStatus.json| |`Invalid` | *FAILURE*: 1 errors, 1 warnings, 0 notes
hl7.fhir.ae-Condition.json| |Valid | Success: 0 errors, 4 warnings, 0 notes
hl7.fhir.ae-Condition-duration.json| |`Invalid` | *FAILURE*: 1 errors, 1 warnings, 0 notes
hl7.fhir.ae-Condition-outcome.json| |`Invalid` | *FAILURE*: 1 errors, 2 warnings, 0 notes
hl7.fhir.ae-Condition-resultingCondition.json| | `Invalid`| *FAILURE*: 1 errors, 1 warnings, 0 notes
hl7.fhir.ae-Condition-seriousness.json| |`Invalid` | *FAILURE*: 1 errors, 1 warnings, 0 notes
hl7.fhir.ae-HumanName.json| | `Invalid`| *FAILURE*: 5 errors, 2 warnings, 0 notes
hl7.fhir.ae-HumanName-salutation.json| |`Invalid` | *FAILURE*: 1 errors, 1 warnings, 0 notes
hl7.fhir.ae-MedicationAdministration.json| | Valid| Success: 0 errors, 6 warnings, 0 notes
hl7.fhir.ae-MedicationAdministration-actionTaken.json| | `Invalid`| *FAILURE*: 1 errors, 1 warnings, 0 notes
hl7.fhir.ae-MedicationAdministration-frequency.json| |`Invalid` | *FAILURE*: 1 errors, 1 warnings, 0 notes
hl7.fhir.ae-MedicationAdministration-operatorDevice.json| |`Invalid` | *FAILURE*: 1 errors, 1 warnings, 0 notes
hl7.fhir.ae-MedicationAdministration-operatorDeviceOther.json| | `Invalid`| *FAILURE*: 1 errors, 1 warnings, 0 notes
hl7.fhir.ae-MedicationAdministration-productType.json| | `Invalid`| *FAILURE*: 1 errors, 1 warnings, 0 notes
hl7.fhir.ae-MedicationAdministration-unit.json| |`Invalid` | *FAILURE*: 1 errors, 1 warnings, 0 notes
hl7.fhir.ae-Observation.json| |Valid | Success: 0 errors, 3 warnings, 0 notes
hl7.fhir.ae-Observation-pregnancyDueDate.json| | `Invalid`| *FAILURE*: 1 errors, 1 warnings, 0 notes
hl7.fhir.ae-Observation-pregnancyFlag.json| | `Invalid`| *FAILURE*: 1 errors, 1 warnings, 0 notes
hl7.fhir.ae-Observation-previousPregnanciesDetails.json| | `Invalid`| *FAILURE*: 1 errors, 1 warnings, 0 notes
hl7.fhir.ae-Patient.json| | `Invalid`| *FAILURE*: 4 errors, 6 warnings, 0 notes
hl7.fhir.ae-Patient-ageGroup.json| | `Invalid`| *FAILURE*: 1 errors, 1 warnings, 0 notes
hl7.fhir.ae-Patient-consentToContactPatient.json| | `Invalid`| *FAILURE*: 1 errors, 1 warnings, 0 notes
hl7.fhir.ae-Patient-ethnicity.json| | `Invalid`| *FAILURE*: 1 errors, 1 warnings, 0 notes
hl7.fhir.ae-Patient-gender.json| | `Invalid`| *FAILURE*: 1 errors, 1 warnings, 0 notes
hl7.fhir.ae-Patient-patientAge.json| |`Invalid` | *FAILURE*: 1 errors, 1 warnings, 0 notes
hl7.fhir.ae-Patient-region.json| | `Invalid`| *FAILURE*: 1 errors, 1 warnings, 0 notes
hl7.fhir.ae-Patient-salutation.json| | `Invalid`| *FAILURE*: 1 errors, 1 warnings, 0 notes
hl7.fhir.ae-Practitioner.json| | `Invalid`| *FAILURE*: 4 errors, 2 warnings, 0 notes
hl7.fhir.ae-Practitioner-consentToContactPractitioner.json| | `Invalid`|*FAILURE*: 1 errors, 1 warnings, 0 notes 
hl7.fhir.ae-Practitioner-region.json| | `Invalid`| *FAILURE*: 1 errors, 1 warnings, 0 notes
hl7.fhir.ae-Practitioner-salutation.json| | `Invalid`| *FAILURE*: 1 errors, 1 warnings, 0 notes
hl7.fhir.ae-RelatedPerson.json| | `Invalid`|Error in snapshot generation 
hl7.fhir.ae-RelatedPerson-consentToContactReporter.json| |`Invalid` | *FAILURE*: 1 errors, 1 warnings, 0 notes
hl7.fhir.ae-RelatedPerson-region.json| | `Invalid`| *FAILURE*: 1 errors, 1 warnings, 0 notes
hl7.fhir.ae-RelatedPerson-salutation.json| |`Invalid` | *FAILURE*: 1 errors, 1 warnings, 0 notes
