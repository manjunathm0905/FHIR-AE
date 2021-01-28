---
title: Documentation
---

# Documentation
---
---

## New Resource Profile Template
---

- description: Text definition of the profile
- name: Name for this structure definition (computer friendly)
- status: The status of this structure definition. Enables tracking the life-cycle of the - content. draft | active | retired | unknown
- fhirVersion: FHIR Version this StructureDefinition targets
- kind: primitive-type | complex-type | resource | logical
- abstract: Whether the structure is abstract (false)
- type: Type defined or constrained by this structure (AdverseEvent)
- baseDefinition: Definition that this type is constrained/specialized from "http://hl7.org/fhir/StructureDefinition/AdverseEvent"
- derivation: specialization | constraint - How relates to base definition - constraint
- title: Name for this structure definition (human friendly) 'AZ AdverseEvent Profile'
- experimental: For testing purposes, not real usage - false
- date: Date last changed "2020-09-30"
- publisher: Name of the publisher (organization or individual) - "AstraZeneca"

- elements:
  - extension:
    - AZEmployeeReporter:
      - type: string
     -  description: AZ Employee Reporter
     -  title: AZ Employee Reporter Extension
     -  experimental: false
     -  date: "2020-12-18"
    -   publisher: AstraZeneca
