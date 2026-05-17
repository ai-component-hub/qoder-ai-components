---
name: 'database-migrations'
description: 'Database migration best practices for schema changes, data migrations,'
adopted: 2026-05-16
batch: bulk-adoption
rollbacks, and zero-downtime deployments across PostgreSQL, MySQL, and common ORMs
(Prisma, Drizzle, Kysely, Django, TypeORM, gol
source: everything-claude-code
---

# database-migrations

Database migration best practices for schema changes, data migrations, rollbacks, and zero-downtime deployments across PostgreSQL, MySQL, and common ORMs (Prisma, Drizzle, Kysely, Django, TypeORM, gol

## When to Use

- Use this skill when working on tasks related to database migrations
- Apply best practices from everything-claude-code

## Workflow

```bash
# Create migration from schema changes
npx prisma migrate dev --name add_user_avatar

# Apply pending migrations in production
npx prisma migrate deploy

# Reset database (dev only)
npx prisma migrate reset

# Generate client after schema changes
npx prisma generate
```

### Schema Example

```prisma
model User {
  id        String   @id @default(cuid())
  email     String   @unique
  name      String?
  avatarUrl String?  @map("avatar_url")
  createdAt DateTime @default(now()) @map("created_at")
  updatedAt DateTime @updatedAt @map("updated_at")
  orders    Order[]

  @@map("users")
  @@index([email])
}
```

### Custom SQL Migration

For operations Prisma cannot express (concurrent indexes, data backfills):

```bash
# Create empty migration, then edit the SQL manually
npx prisma m

## Source

Adopted from: everything-claude-code
