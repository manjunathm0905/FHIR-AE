---
title: Instruction
---

# Instruction

- Clone the repository

- Access the repository folder

- Run the command:

```
java -jar "./igpop/target/igpop.jar" dev -p 8891
```

- Open localhost:8891

- Click the Package link to generate a package of FHIR StractureDefinitions and ValueSets

- The package will be downloaded as a zip-archive

- Unzip the archive

- Browse the folder

- The folder will contain FHIR StractureDefinitions and ValueSets

## StractureDefinitions

**File**|**Status**
-----|-----
hl7.fhir.ae-Address-region.json| Success: 0 errors, 1 warnings, 0 notes
hl7.fhir.ae-Address.json| Success: 0 errors, 1 warnings, 0 notes
hl7.fhir.ae-AdverseEvent-AZEmployeeReporter.json| Success: 0 errors, 0 warnings, 1 notes
hl7.fhir.ae-AdverseEvent-lateReason.json| Success: 0 errors, 1 warnings, 0 notes
hl7.fhir.ae-AdverseEvent-localReference.json| Success: 0 errors, 1 warnings, 0 notes
hl7.fhir.ae-AdverseEvent-positiveDechallenge.json| Success: 0 errors, 1 warnings, 0 notes
hl7.fhir.ae-AdverseEvent-positiveRechallenge.json| Success: 0 errors, 1 warnings, 0 notes
hl7.fhir.ae-AdverseEvent-programNumber.json| Success: 0 errors, 1 warnings, 0 notes
hl7.fhir.ae-AdverseEvent-rechallenge.json| Success: 0 errors, 1 warnings, 0 notes
hl7.fhir.ae-AdverseEvent-reporterType.json| Success: 0 errors, 1 warnings, 0 notes
hl7.fhir.ae-AdverseEvent-sourceType.json| Success: 0 errors, 1 warnings, 0 notes
hl7.fhir.ae-AdverseEvent-surveyStatus.json| Success: 0 errors, 1 warnings, 0 notes
hl7.fhir.ae-AdverseEvent.json| Success: 0 errors, 10 warnings, 0 notes
hl7.fhir.ae-Condition-duration.json| Success: 0 errors, 1 warnings, 0 notes
hl7.fhir.ae-Condition-outcome.json| Success: 0 errors, 1 warnings, 0 notes
hl7.fhir.ae-Condition-resultingCondition.json| Success: 0 errors, 1 warnings, 0 notes
hl7.fhir.ae-Condition-seriousness.json| Success: 0 errors, 1 warnings, 0 notes
hl7.fhir.ae-Condition.json| Success: 0 errors, 4 warnings, 0 notes
hl7.fhir.ae-HumanName-salutation.json| Success: 0 errors, 1 warnings, 0 notes
hl7.fhir.ae-HumanName.json| Success: 0 errors, 1 warnings, 0 notes
hl7.fhir.ae-MedicationAdministration-actionTaken.json| Success: 0 errors, 1 warnings, 0 notes
hl7.fhir.ae-MedicationAdministration-frequency.json| Success: 0 errors, 1 warnings, 0 notes
hl7.fhir.ae-MedicationAdministration-operatorDevice.json| Success: 0 errors, 1 warnings, 0 notes
hl7.fhir.ae-MedicationAdministration-operatorDeviceOther.json| Success: 0 errors, 1 warnings, 0 notes
hl7.fhir.ae-MedicationAdministration-productType.json| Success: 0 errors, 1 warnings, 0 notes
hl7.fhir.ae-MedicationAdministration-unit.json| Success: 0 errors, 1 warnings, 0 notes
hl7.fhir.ae-MedicationAdministration.json| Success: 0 errors, 6 warnings, 0 notes
 hl7.fhir.ae-Observation-pregnancyDueDate.json| Success: 0 errors, 1 warnings, 0 notes
hl7.fhir.ae-Observation-pregnancyFlag.json| Success: 0 errors, 1 warnings, 0 notes
hl7.fhir.ae-Observation-previousPregnanciesDetails.json| Success: 0 errors, 1 warnings, 0 notes
hl7.fhir.ae-Observation.json| Success: 0 errors, 3 warnings, 0 notes
 hl7.fhir.ae-Patient-ageGroup.json| Success: 0 errors, 1 warnings, 0 notes
hl7.fhir.ae-Patient-consentToContactPatient.json| Success: 0 errors, 1 warnings, 0 notes
hl7.fhir.ae-Patient-ethnicity.json| Success: 0 errors, 1 warnings, 0 notes
hl7.fhir.ae-Patient-gender.json| Success: 0 errors, 1 warnings, 0 notes
hl7.fhir.ae-Patient-patientAge.json| Success: 0 errors, 1 warnings, 0 notes
hl7.fhir.ae-Patient.json| *FAILURE*: 2 errors, 5 warnings, 0 notes   Unrecognised property '@profile'  
hl7.fhir.ae-Practitioner-consentToContactPractitioner.json| Success: 0 errors, 1 warnings, 0 notes
hl7.fhir.ae-Practitioner.json| *FAILURE*: 2 errors, 1 warnings, 0 notes   Unrecognised property '@profile' 
hl7.fhir.ae-RelatedPerson-consentToContactReporter.json| Success: 0 errors, 1 warnings, 0 notes
hl7.fhir.ae-RelatedPerson.json| *FAILURE*: 2 errors, 1 warnings, 0 notes   Unrecognised property '@profile'


## ValueSets


**File**|**Status**|**FHIR Validator Output**
-----|-----|-----
hl7.fhir.ae-condition-outcome.json|Success: 0 errors, 1 warnings, 0 notes|Warning @ ValueSet.compose[0].include[0] : Unknown System specified, so Concepts and Filters can't be checked
hl7.fhir.ae-condition-seriousness.json|Success: 0 errors, 1 warnings, 0 notes|Warning @ ValueSet.compose[0].include[0] : Unknown System specified, so Concepts and Filters can't be checked
hl7.fhir.ae-detailed-ethnicity.json|Success: 0 errors, 1 warnings, 0 notes|Warning @ ValueSet.compose[0].include[0] : Unknown System specified, so Concepts and Filters can't be checked
hl7.fhir.ae-intelligent-source.json|Success: 0 errors, 1 warnings, 0 notes|Warning @ ValueSet.compose[0].include[0] : Unknown System specified, so Concepts and Filters can't be checked
hl7.fhir.ae-resulting-condition.json|Success: 0 errors, 1 warnings, 0 notes|Warning @ ValueSet.compose[0].include[0] : Unknown System specified, so Concepts and Filters can't be checked
hl7.fhir.ae-survey-status.json|Success: 0 errors, 1 warnings, 0 notes|Warning @ ValueSet.compose[0].include[0] : Unknown System specified, so Concepts and Filters can't be checked
