---
name: 'healthcare-emr-patterns'
description: 'EMR/EHR development patterns for healthcare applications. Clinical safety,'
adopted: 2026-05-16
encounter workflows, prescription generation, clinical decision support integration,
and accessibility-first UI for medical d
source: everything-claude-code
tier: 2
---

# healthcare-emr-patterns

EMR/EHR development patterns for healthcare applications. Clinical safety, encounter workflows, prescription generation, clinical decision support integration, and accessibility-first UI for medical d

## When to Use

- Use this skill when working on tasks related to healthcare emr patterns
- Trigger when you need expertise in this domain
- Apply best practices from everything-claude-code

## Workflow

name: healthcare-emr-patterns
description: EMR/EHR development patterns for healthcare applications. Clinical safety, encounter workflows, prescription generation, clinical decision support integration, and accessibility-first UI for medical data entry.
origin: Health1 Super Speciality Hospitals — contributed by Dr. Keyur Patel
version: "1.0.0"
# Healthcare EMR Development Patterns
Patterns for building Electronic Medical Record (EMR) and Electronic Health Record (EHR) systems. Prioritizes patient safety, clinical accuracy, and practitioner efficiency.
## When to Use
- Building patient encounter workflows (complaint, exam, diagnosis, prescription)
- Implementing clinical note-taking (structured + free text + voice-to-text)
- Designing prescription/medication modules with drug interaction checking
- Integrating Clinical Decision Support Systems (CDSS)
- Building lab result displays with reference range highlighting
- Implementing audit trails for clinical data
- Designing healthcare-accessible UIs for clinical data entry
## How It Works
### Patient Safety First
Every design decision must be evaluated against: "Could this harm a patient?"
- Drug interactions MUST alert, not silently pass
- Abnormal lab values MUST be visually flagged
- Critical vitals MUST trigger escalation workflows

## Source

This skill was adopted from open-source repository: everything-claude-code
Original path: healthcare-emr-patterns
