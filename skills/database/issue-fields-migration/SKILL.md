---
name: 'issue-fields-migration'
description: 'Bulk-migrate metadata to GitHub issue fields from two sources: repo labels (e.g. priority labels to a Priority field) and Project V2 fields. Use when users say'
version: 1.0.0
source: awesome-copilot
tier: 3
adopted: 2026-05-16
batch: bulk-adoption
---

# issue-fields-migration

'Bulk-migrate metadata to GitHub issue fields from two sources: repo labels (e.g. priority labels to a Priority field) and Project V2 fields. Use when users say "migrate my labels to issue fields", "m

## When to Use

- Use this skill when working on tasks related to issue fields migration
- Apply best practices from awesome-copilot

## Workflow

### Step 0: Migration Source

Ask the user what they are migrating:

1. **"Are you migrating labels or project fields?"**
   - **Labels**: proceed to the [Label Migration Flow](#label-migration-flow) below.
   - **Project fields**: proceed to the [Project Field Migration Flow](#project-field-migration-flow) below.

2. If the user says **labels**:
   - Ask: "Which org and repo(s) contain the labels?"
   - Ask: "Which labels do you want to migrate?" (they can name them or say "show me the labels first")

3. If the user says **project fields**:
   - Ask: "Can you share the link to your project or tell me the org name and project number?"
   - Ask: "Which field do you want to migrate?"

---

### Label Migration Flow

Use this flow when the user wants to convert repo labels into issue field val

## Source

Adopted from: awesome-copilot
