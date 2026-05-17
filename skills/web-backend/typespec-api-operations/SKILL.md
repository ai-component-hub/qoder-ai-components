---
name: 'typespec-api-operations'
description: 'Add GET, POST, PATCH, and DELETE operations to a TypeSpec API plugin'
adopted: 2026-05-16
with proper routing, parameters, and adaptive cards
source: awesome-copilot
tier: 2
version: 1.0.0
---

# typespec-api-operations

'Add GET, POST, PATCH, and DELETE operations to a TypeSpec API plugin with proper routing, parameters, and adaptive cards'

## When to Use

- Use this skill when working on tasks related to typespec api operations
- Trigger when you need expertise in this domain
- Apply best practices from awesome-copilot

## Workflow

name: typespec-api-operations
description: 'Add GET, POST, PATCH, and DELETE operations to a TypeSpec API plugin with proper routing, parameters, and adaptive cards'
# Add TypeSpec API Operations
Add RESTful operations to an existing TypeSpec API plugin for Microsoft 365 Copilot.
## Adding GET Operations
### Simple GET - List All Items
```typescript
/**
 * List all items.
 */
@route("/items")
@get op listItems(): Item[];
```
### GET with Query Parameter - Filter Results
```typescript
/**
 * List items filtered by criteria.
 * @param userId Optional user ID to filter items
 */
@route("/items")

## Source

This skill was adopted from open-source repository: awesome-copilot
Original path: typespec-api-operations
