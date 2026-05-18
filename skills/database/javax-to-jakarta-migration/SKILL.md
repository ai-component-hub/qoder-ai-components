---
name: 'javax-to-jakarta-migration'
description: 'Migrate Java code from javax.* to jakarta.* namespace. Use when upgrading'
adopted: 2026-05-16
batch: bulk-adoption
to Tomcat 11, Jakarta EE 10, or when javax imports are detected in the codebase.
source: awesome-copilot
tier: 3
---

# javax-to-jakarta-migration

"Migrate Java code from javax.* to jakarta.* namespace. Use when upgrading to Tomcat 11, Jakarta EE 10, or when javax imports are detected in the codebase."

## When to Use

- Use this skill when working on tasks related to javax to jakarta migration
- Apply best practices from awesome-copilot

## Workflow

name: javax-to-jakarta-migration
description: "Migrate Java code from javax.* to jakarta.* namespace. Use when upgrading to Tomcat 11, Jakarta EE 10, or when javax imports are detected in the codebase."
argument-hint: "File, package, or module to migrate"
# javax → jakarta Migration Skill
## When to Use
- Upgrading to Tomcat 11 / Jakarta EE 10+
- Code review detects `javax.*` imports
- Migrating an existing project to the jakarta namespace
## Procedure
### Step 1 — Scan for javax Usage
Search the codebase for all `javax.*` imports that need migration:
```
javax.servlet.*      → jakarta.servlet

## Source

Adopted from: awesome-copilot
