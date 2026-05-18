---
name: 'domain-driven-design'
description: 'Plan and route Domain-Driven Design work from strategic modeling to tactical'
adopted: 2026-05-16
batch: bulk-adoption
implementation and evented architecture patterns.
source: antigravity-awesome-skills
tier: 4
---

# domain-driven-design

"Plan and route Domain-Driven Design work from strategic modeling to tactical implementation and evented architecture patterns."

## When to Use

- Use this skill when working on tasks related to domain driven design
- Apply best practices from antigravity-awesome-skills

## Workflow

1. Run a viability check before committing to full DDD.
2. Produce strategic artifacts first: subdomains, bounded contexts, language glossary.
3. Route to specialized skills based on current task.
4. Define success criteria and evidence for each stage.

### Viability check

Use full DDD only when at least two of these are true:

- Business rules are complex or fast-changing.
- Multiple teams are causing model collisions.
- Integration contracts are unstable.
- Auditability and explicit invariants are critical.

### Routing map

- Strategic model and boundaries: `@ddd-strategic-design`
- Cross-context integrations and translation: `@ddd-context-mapping`
- Tactical code modeling: `@ddd-tactical-patterns`
- Read/write separation: `@cqrs-implementation`
- Event history as source of truth: `@ev

## Source

Adopted from: antigravity-awesome-skills
