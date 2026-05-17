---
name: 'fastapi-patterns'
description: 'FastAPI patterns for async APIs, dependency injection, Pydantic request'
adopted: 2026-05-16
and response models, OpenAPI docs, tests, security, and production readiness.
source: everything-claude-code
tier: 2
version: 1.0.0
---

# fastapi-patterns

FastAPI patterns for async APIs, dependency injection, Pydantic request and response models, OpenAPI docs, tests, security, and production readiness.

## When to Use

- Use this skill when working on tasks related to fastapi patterns
- Trigger when you need expertise in this domain
- Apply best practices from everything-claude-code

## Workflow

name: fastapi-patterns
description: FastAPI patterns for async APIs, dependency injection, Pydantic request and response models, OpenAPI docs, tests, security, and production readiness.
origin: community
# FastAPI Patterns
Production-oriented patterns for FastAPI services.
## When to Use
- Building or reviewing a FastAPI app.
- Splitting routers, schemas, dependencies, and database access.
- Writing async endpoints that call a database or external service.
- Adding authentication, authorization, OpenAPI docs, tests, or deployment settings.
- Checking a FastAPI PR for copy-pasteable examples and production risks.
## How It Works
Treat the FastAPI app as a thin HTTP layer over explicit dependencies and service code:
- `main.py` owns app construction, middleware, exception handlers, and router registration.
- `schemas/` owns Pydantic request and response models.
- `dependencies.py` owns database, auth, pagination, and request-scoped dependencies.
- `services/` or `crud/` owns business and persistence operations.
- `tests/` overrides dependencies instead of opening production resources.
Prefer small routers and explicit `response_model` declarations. Keep raw ORM objects, secrets, and framework globals out of response schemas.
## Project Layout

## Source

This skill was adopted from open-source repository: everything-claude-code
Original path: fastapi-patterns
