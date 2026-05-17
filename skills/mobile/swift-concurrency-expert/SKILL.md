---
name: 'swift-concurrency-expert'
description: 'Review and fix Swift concurrency issues such as actor isolation and Sendable'
adopted: 2026-05-16
batch: bulk-adoption
violations.
source: antigravity-awesome-skills
tier: 4
---

# swift-concurrency-expert

Review and fix Swift concurrency issues such as actor isolation and Sendable violations.

## When to Use

- Use this skill when working on tasks related to swift concurrency expert
- Apply best practices from antigravity-awesome-skills

## Workflow

### 1. Triage the issue

- Capture the exact compiler diagnostics and the offending symbol(s).
- Check project concurrency settings: Swift language version (6.2+), strict concurrency level, and whether approachable concurrency (default actor isolation / main-actor-by-default) is enabled.
- Identify the current actor context (`@MainActor`, `actor`, `nonisolated`) and whether a default actor isolation mode is enabled.
- Confirm whether the code is UI-bound or intended to run off the main actor.

### 2. Apply the smallest safe fix

Prefer edits that preserve existing behavior while satisfying data-race safety.

Common fixes:
- **UI-bound types**: annotate the type or relevant members with `@MainActor`.
- **Protocol conformance on main actor types**: make the conformance isolated (e.g., `exten

## Source

Adopted from: antigravity-awesome-skills
