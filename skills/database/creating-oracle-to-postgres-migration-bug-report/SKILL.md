---
name: 'creating-oracle-to-postgres-migration-bug-report'
description: 'Creates structured bug reports for defects found during Oracle-to-PostgreSQL migration. Use when documenting behavioral differences between Oracle and PostgreSQL as actionable bug reports with severi'
version: 1.0.0
source: awesome-copilot
tier: 2
adopted: 2026-05-16
---

# creating-oracle-to-postgres-migration-bug-report

'Creates structured bug reports for defects found during Oracle-to-PostgreSQL migration. Use when documenting behavioral differences between Oracle and PostgreSQL as actionable bug reports with severi

## When to Use

- Use this skill when working on tasks related to creating oracle to postgres migration bug report
- Trigger when you need expertise in this domain
- Apply best practices from awesome-copilot

## Workflow

name: creating-oracle-to-postgres-migration-bug-report
description: 'Creates structured bug reports for defects found during Oracle-to-PostgreSQL migration. Use when documenting behavioral differences between Oracle and PostgreSQL as actionable bug reports with severity, root cause, and remediation steps.'
# Creating Bug Reports for Oracle-to-PostgreSQL Migration
## When to Use
- Documenting a defect caused by behavioral differences between Oracle and PostgreSQL
- Writing or reviewing a bug report for an Oracle-to-PostgreSQL migration project
## Bug Report Format
Use the template in [references/BUG-REPORT-TEMPLATE.md](references/BUG-REPORT-TEMPLATE.md). Each report must include:
- **Status**: ✅ RESOLVED, ⛔ UNRESOLVED, or ⏳ IN PROGRESS
- **Component**: Affected endpoint, repository, or stored procedure
- **Test**: Related automated test names
- **Severity**: Low / Medium / High / Critical — based on impact scope
- **Problem**: Expected Oracle behavior vs. observed PostgreSQL behavior
- **Scenario**: Ordered reproduction steps with seed data, operation, expected result, and actual result
- **Root Cause**: The specific Oracle/PostgreSQL behavioral difference causing the defect
- **Solution**: Changes made or required, with explicit file paths
- **Validation**: Steps to confirm the fix on both databases
## Oracle-to-PostgreSQL Guidance
- **Oracle is the source of truth** — frame expected behavior from the Oracle baseline
- Call out data layer nuances explicitly: empty string vs. NULL, type coercion strictness, collation, sequence values, time zones, padding, constraints

## Source

This skill was adopted from open-source repository: awesome-copilot
Original path: creating-oracle-to-postgres-migration-bug-report
