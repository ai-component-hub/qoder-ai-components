---
name: 'healthcare-eval-harness'
description: 'Patient safety evaluation harness for healthcare application deployments.'
adopted: 2026-05-16
Automated test suites for CDSS accuracy, PHI exposure, clinical workflow integrity,
and integration compliance. Blocks deploym
source: everything-claude-code
tier: 2
---

# healthcare-eval-harness

Patient safety evaluation harness for healthcare application deployments. Automated test suites for CDSS accuracy, PHI exposure, clinical workflow integrity, and integration compliance. Blocks deploym

## When to Use

- Use this skill when working on tasks related to healthcare eval harness
- Trigger when you need expertise in this domain
- Apply best practices from everything-claude-code

## Workflow

name: healthcare-eval-harness
description: Patient safety evaluation harness for healthcare application deployments. Automated test suites for CDSS accuracy, PHI exposure, clinical workflow integrity, and integration compliance. Blocks deployments on safety failures.
origin: Health1 Super Speciality Hospitals — contributed by Dr. Keyur Patel
version: "1.0.0"
# Healthcare Eval Harness — Patient Safety Verification
Automated verification system for healthcare application deployments. A single CRITICAL failure blocks deployment. Patient safety is non-negotiable.
> **Note:** Examples use Jest as the reference test runner. Adapt commands for your framework (Vitest, pytest, PHPUnit, etc.) — the test categories and pass thresholds are framework-agnostic.
## When to Use
- Before any deployment of EMR/EHR applications
- After modifying CDSS logic (drug interactions, dose validation, scoring)
- After changing database schemas that touch patient data
- After modifying authentication or access control
- During CI/CD pipeline configuration for healthcare apps
- After resolving merge conflicts in clinical modules
## How It Works
The eval harness runs five test categories in order. The first three (CDSS Accuracy, PHI Exposure, Data Integrity) are CRITICAL gates requiring 100% pass rate — a single failure blocks deployment. The remaining two (Clinical Workflow, Integration) are HIGH gates requiring 95%+ pass rate.
Each category maps to a Jest test path pattern. The CI pipeline runs CRITICAL gates with `--bail` (stop on first failure) and enforces coverage thresholds with `--coverage --coverageThreshold`.
### Eval Categories
**1. CDSS Accuracy (CRITICAL — 100% required)**
Tests all clinical decision support logic: drug interaction pairs (both directions), dose validation rules, clinical scoring vs published specs, no false negatives, no silent failures.

## Source

This skill was adopted from open-source repository: everything-claude-code
Original path: healthcare-eval-harness
