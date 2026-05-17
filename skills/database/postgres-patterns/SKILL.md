---
name: 'postgres-patterns'
description: 'PostgreSQL database patterns for query optimization, schema design, indexing,'
adopted: 2026-05-16
and security. Based on Supabase best practices.
source: everything-claude-code
tier: 2
version: 1.0.0
---

# postgres-patterns

PostgreSQL database patterns for query optimization, schema design, indexing, and security. Based on Supabase best practices.

## When to Use

- Use this skill when working on tasks related to postgres patterns
- Trigger when you need expertise in this domain
- Apply best practices from everything-claude-code

## Workflow

name: postgres-patterns
description: PostgreSQL database patterns for query optimization, schema design, indexing, and security. Based on Supabase best practices.
origin: ECC
# PostgreSQL Patterns
Quick reference for PostgreSQL best practices. For detailed guidance, use the `database-reviewer` agent.
## When to Activate
- Writing SQL queries or migrations
- Designing database schemas
- Troubleshooting slow queries
- Implementing Row Level Security
- Setting up connection pooling
## Quick Reference
### Index Cheat Sheet
| Query Pattern | Index Type | Example |
|--------------|------------|---------|
| `WHERE col = value` | B-tree (default) | `CREATE INDEX idx ON t (col)` |
| `WHERE col > value` | B-tree | `CREATE INDEX idx ON t (col)` |
| `WHERE a = x AND b > y` | Composite | `CREATE INDEX idx ON t (a, b)` |
| `WHERE jsonb @> '{}'` | GIN | `CREATE INDEX idx ON t USING gin (col)` |
| `WHERE tsv @@ query` | GIN | `CREATE INDEX idx ON t USING gin (col)` |

## Source

This skill was adopted from open-source repository: everything-claude-code
Original path: postgres-patterns
