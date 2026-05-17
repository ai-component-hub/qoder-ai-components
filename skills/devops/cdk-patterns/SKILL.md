---
name: 'cdk-patterns'
description: 'Common AWS CDK patterns and constructs for building cloud infrastructure'
adopted: 2026-05-16
batch: bulk-adoption
with TypeScript, Python, or Java. Use when designing reusable CDK stacks and L3
constructs.
source: antigravity-awesome-skills
---

# cdk-patterns

"Common AWS CDK patterns and constructs for building cloud infrastructure with TypeScript, Python, or Java. Use when designing reusable CDK stacks and L3 constructs."

## When to Use

- Use this skill when working on tasks related to cdk patterns
- Apply best practices from antigravity-awesome-skills

## Workflow

1. Identify the infrastructure pattern needed (e.g., serverless API, container service, data pipeline).
2. Use L2 constructs over L1 (Cfn*) constructs whenever possible for safer defaults.
3. Apply the principle of least privilege for all IAM roles and policies.
4. Use `RemovalPolicy` and `Tags` appropriately for production readiness.
5. Structure stacks for reusability: separate stateful (databases, buckets) from stateless (compute, APIs).
6. Enable monitoring by default (CloudWatch alarms, X-Ray tracing).

## Source

Adopted from: antigravity-awesome-skills
