---
name: 'scaffolding-oracle-to-postgres-migration-test-project'
description: 'Scaffolds an xUnit integration test project for validating Oracle-to-PostgreSQL database migration behavior in .NET solutions. Creates the test project, transaction-rollback base class, and seed data'
version: 1.0.0
source: awesome-copilot
tier: 3
adopted: 2026-05-16
batch: bulk-adoption
---

# scaffolding-oracle-to-postgres-migration-test-project

'Scaffolds an xUnit integration test project for validating Oracle-to-PostgreSQL database migration behavior in .NET solutions. Creates the test project, transaction-rollback base class, and seed data

## When to Use

- Use this skill when working on tasks related to scaffolding oracle to postgres migration test project
- Apply best practices from awesome-copilot

## Workflow

```
Progress:
- [ ] Step 1: Inspect the target project
- [ ] Step 2: Create the xUnit test project
- [ ] Step 3: Implement transaction-rollback base class
- [ ] Step 4: Implement seed data manager
- [ ] Step 5: Verify the project compiles
```

**Step 1: Inspect the target project**

Read the target project's `.csproj` to determine the .NET version and existing package references. Match these versions exactly — do not upgrade.

**Step 2: Create the xUnit test project**

- Target the same .NET version as the application under test.
- Add NuGet packages for Oracle database connectivity and xUnit.
- Add a project reference to the target project only — no other application projects.
- Add an `appsettings.json` configured for Oracle database connectivity.

**Step 3: Implement transaction-rollbac

## Source

Adopted from: awesome-copilot
