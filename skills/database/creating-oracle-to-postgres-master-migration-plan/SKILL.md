---
name: 'creating-oracle-to-postgres-master-migration-plan'
description: 'Discovers all projects in a .NET solution, classifies each for Oracle-to-PostgreSQL migration eligibility, and produces a persistent master migration plan. Use when starting a multi-project Oracle-to'
version: 1.0.0
source: awesome-copilot
tier: 3
adopted: 2026-05-16
batch: bulk-adoption
---

# creating-oracle-to-postgres-master-migration-plan

'Discovers all projects in a .NET solution, classifies each for Oracle-to-PostgreSQL migration eligibility, and produces a persistent master migration plan. Use when starting a multi-project Oracle-to

## When to Use

- Use this skill when working on tasks related to creating oracle to postgres master migration plan
- Apply best practices from awesome-copilot

## Workflow

```
Progress:
- [ ] Step 1: Discover projects in the solution
- [ ] Step 2: Classify each project
- [ ] Step 3: Confirm with user
- [ ] Step 4: Write the plan file
```

**Step 1: Discover projects**

Find the Solution File (it has a `.sln` or `.slnx` extension) in the workspace root (ask the user if multiple exist). Parse it to extract all `.csproj` project references. For each project, note the name, path, and type (class library, web API, console, test, etc.).

**Step 2: Classify each project**

Scan every non-test project for Oracle indicators:

- NuGet references: `Oracle.ManagedDataAccess`, `Oracle.EntityFrameworkCore` (check `.csproj` and `packages.config`)
- Config entries: Oracle connection strings in `appsettings.json`, `web.config`, `app.config`
- Code usage: `OracleConnection`, 

## Source

Adopted from: awesome-copilot
