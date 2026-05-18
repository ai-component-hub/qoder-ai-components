---
name: 'agent-harness-construction'
description: 'Design and optimize AI agent action spaces, tool definitions, and observation'
adopted: 2026-05-16
formatting for higher completion rates.
source: everything-claude-code
tier: 2
version: 1.0.0
---

# agent-harness-construction

Design and optimize AI agent action spaces, tool definitions, and observation formatting for higher completion rates.

## When to Use

- Use this skill when working on tasks related to agent harness construction
- Trigger when you need expertise in this domain
- Apply best practices from everything-claude-code

## Workflow

name: agent-harness-construction
description: Design and optimize AI agent action spaces, tool definitions, and observation formatting for higher completion rates.
origin: ECC
# Agent Harness Construction
Use this skill when you are improving how an agent plans, calls tools, recovers from errors, and converges on completion.
## Core Model
Agent output quality is constrained by:
1. Action space quality
2. Observation quality
3. Recovery quality
4. Context budget quality
## Action Space Design
1. Use stable, explicit tool names.
2. Keep inputs schema-first and narrow.
3. Return deterministic output shapes.
4. Avoid catch-all tools unless isolation is impossible.
## Granularity Rules
- Use micro-tools for high-risk operations (deploy, migration, permissions).
- Use medium tools for common edit/read/search loops.
- Use macro-tools only when round-trip overhead is the dominant cost.

## Source

This skill was adopted from open-source repository: everything-claude-code
Original path: agent-harness-construction
