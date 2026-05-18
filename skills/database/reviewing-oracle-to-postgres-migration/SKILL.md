---
name: 'reviewing-oracle-to-postgres-migration'
description: 'Identifies Oracle-to-PostgreSQL migration risks by cross-referencing code against known behavioral differences (empty strings, refcursors, type coercion, sorting, timestamps, concurrent transactions,'
version: 1.0.0
source: awesome-copilot
tier: 3
adopted: 2026-05-16
batch: bulk-adoption
---

# reviewing-oracle-to-postgres-migration

'Identifies Oracle-to-PostgreSQL migration risks by cross-referencing code against known behavioral differences (empty strings, refcursors, type coercion, sorting, timestamps, concurrent transactions,

## When to Use

- Use this skill when working on tasks related to reviewing oracle to postgres migration
- Apply best practices from awesome-copilot

## Workflow

Determine the task type:

**Planning a migration?** Follow the risk assessment workflow.
**Validating completed work?** Follow the validation workflow.

### Risk assessment workflow (planning)

```
Risk Assessment:
- [ ] Step 1: Identify the migration scope
- [ ] Step 2: Screen each insight for applicability
- [ ] Step 3: Document risks and recommended actions
```

**Step 1: Identify the migration scope**

List the affected database objects (procedures, triggers, queries, views) and the application code that calls them.

**Step 2: Screen each insight for applicability**

Review the reference index in [references/REFERENCE.md](references/REFERENCE.md). For each entry, determine whether the migration scope contains patterns affected by that insight. Read the full reference file only when the

## Source

Adopted from: awesome-copilot
