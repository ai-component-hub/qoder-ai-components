---
name: 'terraform-aws-modules'
description: 'Terraform module creation for AWS — reusable modules, state management,'
adopted: 2026-05-16
batch: bulk-adoption
and HCL best practices. Use when building or reviewing Terraform AWS infrastructure.
source: antigravity-awesome-skills
tier: 4
---

# terraform-aws-modules

"Terraform module creation for AWS — reusable modules, state management, and HCL best practices. Use when building or reviewing Terraform AWS infrastructure."

## When to Use

- Use this skill when working on tasks related to terraform aws modules
- Apply best practices from antigravity-awesome-skills

## Workflow

1. Structure modules with clear `variables.tf`, `outputs.tf`, `main.tf`, and `versions.tf`.
2. Pin provider and module versions to avoid breaking changes.
3. Use remote state (S3 + DynamoDB locking) for team environments.
4. Apply `terraform fmt` and `terraform validate` before commits.
5. Use `for_each` over `count` for resources that need stable identity.
6. Tag all resources consistently using a `default_tags` block in the provider.

## Source

Adopted from: antigravity-awesome-skills
