---
name: 'api-connector-builder'
description: 'Build a new API connector or provider by matching the target repo'
adopted: 2026-05-16
batch: bulk-adoption
integration pattern exactly. Use when adding one more integration without inventing
a second architecture.
source: everything-claude-code
---

# api-connector-builder

Build a new API connector or provider by matching the target repo's existing integration pattern exactly. Use when adding one more integration without inventing a second architecture.

## When to Use

- Use this skill when working on tasks related to api connector builder
- Apply best practices from everything-claude-code

## Workflow

### 1. Learn the house style

Inspect at least 2 existing connectors/providers and map:

- file layout
- abstraction boundaries
- config model
- retry / pagination conventions
- registry hooks
- test fixtures and naming

### 2. Narrow the target integration

Define only the surface the repo actually needs:

- auth flow
- key entities
- core read/write operations
- pagination and rate limits
- webhook or polling model

### 3. Build in repo-native layers

Typical slices:

- config/schema
- client/transport
- mapping layer
- connector/provider entrypoint
- registration
- tests

### 4. Validate against the source pattern

The new connector should look obvious in the codebase, not imported from a different ecosystem.

## Source

Adopted from: everything-claude-code
