---
name: 'creating-oracle-to-postgres-migration-integration-tests'
description: 'Creates integration test cases for .NET data access artifacts during Oracle-to-PostgreSQL database migrations. Generates DB-agnostic xUnit tests with deterministic seed data that validate behavior co'
version: 1.0.0
source: awesome-copilot
tier: 3
adopted: 2026-05-16
batch: bulk-adoption
---

# creating-oracle-to-postgres-migration-integration-tests

'Creates integration test cases for .NET data access artifacts during Oracle-to-PostgreSQL database migrations. Generates DB-agnostic xUnit tests with deterministic seed data that validate behavior co

## When to Use

- Use this skill when working on tasks related to creating oracle to postgres migration integration tests
- Apply best practices from awesome-copilot

## Workflow

```
Test Creation:
- [ ] Step 1: Discover the test project conventions
- [ ] Step 2: Identify testable data access artifacts
- [ ] Step 3: Create seed data
- [ ] Step 4: Write test cases
- [ ] Step 5: Review determinism
```

**Step 1: Discover the test project conventions**

Read the base test class, seed manager, and project file to understand inheritance patterns, transaction management, and seed file conventions.

**Step 2: Identify testable data access artifacts**

Scope to the target project only. List data access methods that interact with the database — repositories, DAOs, stored procedure callers, query builders.

**Step 3: Create seed data**

- Follow seed file location and naming conventions from the existing project.
- Reuse existing seed files when possible.
- Avoid `TRUNCATE T

## Source

Adopted from: awesome-copilot
