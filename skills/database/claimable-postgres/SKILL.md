---
name: 'claimable-postgres'
description: 'Provision instant temporary Postgres databases via Claimable Postgres'
adopted: 2026-05-16
batch: bulk-adoption
by Neon (pg.new). No login or credit card required. Use for quick Postgres environments
and throwaway DATABASE_URL for prototyping
source: antigravity-awesome-skills
---

# claimable-postgres

Provision instant temporary Postgres databases via Claimable Postgres by Neon (pg.new). No login or credit card required. Use for quick Postgres environments and throwaway DATABASE_URL for prototyping

## When to Use

- Use this skill when working on tasks related to claimable postgres
- Apply best practices from antigravity-awesome-skills

## Workflow

name: claimable-postgres
description: Provision instant temporary Postgres databases via Claimable Postgres by Neon (pg.new). No login or credit card required. Use for quick Postgres environments and throwaway DATABASE_URL for prototyping.
risk: unknown
source: community
# Claimable Postgres
Instant Postgres databases for local development, demos, prototyping, and test environments. No account required. Databases expire after 72 hours unless claimed to a Neon account.
## Quick Start
```bash
curl -s -X POST "https://pg.new/api/v1/database" \
  -H "Content-Type: application/json" \
  -d '{"ref":

## Source

Adopted from: antigravity-awesome-skills
