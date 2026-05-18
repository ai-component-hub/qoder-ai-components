---
name: 'prisma-patterns'
description: 'Prisma ORM patterns for TypeScript backends — schema design, query optimization,'
adopted: 2026-05-16
batch: bulk-adoption
transactions, pagination, and critical traps like updateMany returning count not
records, $transaction timeouts, migrat
source: everything-claude-code
---

# prisma-patterns

Prisma ORM patterns for TypeScript backends — schema design, query optimization, transactions, pagination, and critical traps like updateMany returning count not records, $transaction timeouts, migrat

## When to Use

- Use this skill when working on tasks related to prisma patterns
- Apply best practices from everything-claude-code

## Workflow

name: prisma-patterns
description: Prisma ORM patterns for TypeScript backends — schema design, query optimization, transactions, pagination, and critical traps like updateMany returning count not records, $transaction timeouts, migrate dev resetting the DB, @updatedAt skipped on bulk writes, and serverless connection exhaustion.
origin: ECC
# Prisma Patterns
Production patterns and non-obvious traps for Prisma ORM in TypeScript backends.
Tested against Prisma 5.x and 6.x. Some behaviors differ from Prisma 4.
Check the Prisma version before applying version-specific patterns:
```bash
npx prism

## Source

Adopted from: everything-claude-code
