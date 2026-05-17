---
name: 'planning-oracle-to-postgres-migration-integration-testing'
description: 'Creates an integration testing plan for .NET data access artifacts during Oracle-to-PostgreSQL database migrations. Analyzes a single project to identify repositories, DAOs, and service layers that i'
version: 1.0.0
source: awesome-copilot
tier: 3
adopted: 2026-05-16
batch: bulk-adoption
---

# planning-oracle-to-postgres-migration-integration-testing

'Creates an integration testing plan for .NET data access artifacts during Oracle-to-PostgreSQL database migrations. Analyzes a single project to identify repositories, DAOs, and service layers that i

## When to Use

- Use this skill when working on tasks related to planning oracle to postgres migration integration testing
- Apply best practices from awesome-copilot

## Workflow

```
Progress:
- [ ] Step 1: Identify data access artifacts
- [ ] Step 2: Classify testing priorities
- [ ] Step 3: Write the testing plan
```

**Step 1: Identify data access artifacts**

Scope to the target project only. Find classes and methods that interact directly with the database — repositories, DAOs, stored procedure callers, service layers performing CRUD operations.

**Step 2: Classify testing priorities**

Rank artifacts by migration risk. Prioritize methods that use Oracle-specific features (refcursors, `TO_CHAR`, implicit type coercion, `NO_DATA_FOUND`) over simple CRUD.

**Step 3: Write the testing plan**

Write a markdown plan covering:
- List of testable artifacts with method signatures
- Recommended test cases per artifact
- Seed data requirements
- Known Oracle→PostgreSQL 

## Source

Adopted from: awesome-copilot
