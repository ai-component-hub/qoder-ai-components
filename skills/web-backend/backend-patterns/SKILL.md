---
name: 'backend-patterns'
description: 'Backend architecture patterns, API design, database optimization, and'
adopted: 2026-05-16
server-side best practices for Node.js, Express, and Next.js API routes.
source: everything-claude-code
tier: 2
version: 1.0.0
---

# backend-patterns

Backend architecture patterns, API design, database optimization, and server-side best practices for Node.js, Express, and Next.js API routes.

## When to Use

- Use this skill when working on tasks related to backend patterns
- Trigger when you need expertise in this domain
- Apply best practices from everything-claude-code

## Workflow

name: backend-patterns
description: Backend architecture patterns, API design, database optimization, and server-side best practices for Node.js, Express, and Next.js API routes.
origin: ECC
# Backend Development Patterns
Backend architecture patterns and best practices for scalable server-side applications.
## When to Activate
- Designing REST or GraphQL API endpoints
- Implementing repository, service, or controller layers
- Optimizing database queries (N+1, indexing, connection pooling)
- Adding caching (Redis, in-memory, HTTP cache headers)
- Setting up background jobs or async processing
- Structuring error handling and validation for APIs
- Building middleware (auth, logging, rate limiting)
## API Design Patterns
### RESTful API Structure
```typescript
// PASS: Resource-based URLs
GET    /api/markets                 # List resources
GET    /api/markets/:id             # Get single resource
POST   /api/markets                 # Create resource

## Source

This skill was adopted from open-source repository: everything-claude-code
Original path: backend-patterns
