---
name: 'cloudformation-best-practices'
description: 'CloudFormation template optimization, nested stacks, drift detection,'
adopted: 2026-05-16
batch: bulk-adoption
and production-ready patterns. Use when writing or reviewing CF templates.
source: antigravity-awesome-skills
tier: 4
---

# cloudformation-best-practices

"CloudFormation template optimization, nested stacks, drift detection, and production-ready patterns. Use when writing or reviewing CF templates."

## When to Use

- Use this skill when working on tasks related to cloudformation best practices
- Apply best practices from antigravity-awesome-skills

## Workflow

1. Use YAML over JSON for readability.
2. Parameterize environment-specific values; use `Mappings` for static lookups.
3. Apply `DeletionPolicy: Retain` on stateful resources (RDS, S3, DynamoDB).
4. Use `Conditions` to support multi-environment templates.
5. Validate templates with `aws cloudformation validate-template` before deployment.
6. Prefer `!Sub` over `!Join` for string interpolation.

## Source

Adopted from: antigravity-awesome-skills
