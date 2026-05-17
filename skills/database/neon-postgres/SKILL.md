---
name: 'neon-postgres'
description: 'Expert patterns for Neon serverless Postgres, branching, connection'
adopted: 2026-05-16
batch: bulk-adoption
source: antigravity-awesome-skills
tier: 4
version: 1.0.0
---

# neon-postgres

Expert patterns for Neon serverless Postgres, branching, connection

## When to Use

- Use this skill when working on tasks related to neon postgres
- Apply best practices from antigravity-awesome-skills

## Workflow

name: neon-postgres
description: Expert patterns for Neon serverless Postgres, branching, connection
  pooling, and Prisma/Drizzle integration
risk: safe
source: vibeship-spawner-skills (Apache 2.0)
date_added: 2026-02-27
# Neon Postgres
Expert patterns for Neon serverless Postgres, branching, connection pooling, and Prisma/Drizzle integration
## Patterns
### Prisma with Neon Connection
Configure Prisma for Neon with connection pooling.
Use two connection strings:
- DATABASE_URL: Pooled connection for Prisma Client
- DIRECT_URL: Direct connection for Prisma Migrate
The pooled connection uses P

## Source

Adopted from: antigravity-awesome-skills
