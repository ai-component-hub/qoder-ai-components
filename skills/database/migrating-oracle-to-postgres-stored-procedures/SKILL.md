---
name: 'migrating-oracle-to-postgres-stored-procedures'
description: 'Migrates Oracle PL/SQL stored procedures to PostgreSQL PL/pgSQL. Translates Oracle-specific syntax, preserves method signatures and type-anchored parameters, leverages orafce where appropriate, and a'
version: 1.0.0
source: awesome-copilot
tier: 3
adopted: 2026-05-16
batch: bulk-adoption
---

# migrating-oracle-to-postgres-stored-procedures

'Migrates Oracle PL/SQL stored procedures to PostgreSQL PL/pgSQL. Translates Oracle-specific syntax, preserves method signatures and type-anchored parameters, leverages orafce where appropriate, and a

## When to Use

- Use this skill when working on tasks related to migrating oracle to postgres stored procedures
- Apply best practices from awesome-copilot

## Workflow

```
Progress:
- [ ] Step 1: Read the Oracle source procedure
- [ ] Step 2: Translate to PostgreSQL PL/pgSQL
- [ ] Step 3: Write the migrated procedure to Postgres output directory
```

**Step 1: Read the Oracle source procedure**

Read the Oracle stored procedure from `.github/oracle-to-postgres-migration/DDL/Oracle/Procedures and Functions/`. Consult the Oracle table/view definitions at `.github/oracle-to-postgres-migration/DDL/Oracle/Tables and Views/` for type resolution.

**Step 2: Translate to PostgreSQL PL/pgSQL**

Apply these translation rules:

- Translate all Oracle-specific syntax to PostgreSQL equivalents.
- Preserve original functionality and control flow logic.
- Keep type-anchored input parameters (e.g., `PARAM_NAME IN table_name.column_name%TYPE`).
- Use explicit types (`NUM

## Source

Adopted from: awesome-copilot
