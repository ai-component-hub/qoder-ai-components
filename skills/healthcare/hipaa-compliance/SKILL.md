---
name: 'hipaa-compliance'
description: 'HIPAA-specific entrypoint for healthcare privacy and security work. Use'
adopted: 2026-05-16
when a task is explicitly framed around HIPAA, PHI handling, covered entities, BAAs,
breach posture, or US healthcare compliance
source: everything-claude-code
tier: 2
---

# hipaa-compliance

HIPAA-specific entrypoint for healthcare privacy and security work. Use when a task is explicitly framed around HIPAA, PHI handling, covered entities, BAAs, breach posture, or US healthcare compliance

## When to Use

- Use this skill when working on tasks related to hipaa compliance
- Trigger when you need expertise in this domain
- Apply best practices from everything-claude-code

## Workflow

name: hipaa-compliance
description: HIPAA-specific entrypoint for healthcare privacy and security work. Use when a task is explicitly framed around HIPAA, PHI handling, covered entities, BAAs, breach posture, or US healthcare compliance requirements.
origin: ECC direct-port adaptation
version: "1.0.0"
# HIPAA Compliance
Use this as the HIPAA-specific entrypoint when a task is clearly about US healthcare compliance. This skill intentionally stays thin and canonical:
- `healthcare-phi-compliance` remains the primary implementation skill for PHI/PII handling, data classification, audit logging, encryption, and leak prevention.
- `healthcare-reviewer` remains the specialized reviewer when code, architecture, or product behavior needs a healthcare-aware second pass.
- `security-review` still applies for general auth, input-handling, secrets, API, and deployment hardening.
## When to Use
- The request explicitly mentions HIPAA, PHI, covered entities, business associates, or BAAs
- Building or reviewing US healthcare software that stores, processes, exports, or transmits PHI
- Assessing whether logging, analytics, LLM prompts, storage, or support workflows create HIPAA exposure
- Designing patient-facing or clinician-facing systems where minimum necessary access and auditability matter
## How It Works
Treat HIPAA as an overlay on top of the broader healthcare privacy skill:
1. Start with `healthcare-phi-compliance` for the concrete implementation rules.
2. Apply HIPAA-specific decision gates:
   - Is this data PHI?
   - Is this actor a covered entity or business associate?

## Source

This skill was adopted from open-source repository: everything-claude-code
Original path: hipaa-compliance
