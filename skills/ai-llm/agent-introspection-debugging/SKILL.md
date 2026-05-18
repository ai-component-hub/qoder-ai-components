---
name: 'agent-introspection-debugging'
description: 'Structured self-debugging workflow for AI agent failures using capture,'
adopted: 2026-05-16
batch: bulk-adoption
diagnosis, contained recovery, and introspection reports.
source: everything-claude-code
tier: 3
---

# agent-introspection-debugging

Structured self-debugging workflow for AI agent failures using capture, diagnosis, contained recovery, and introspection reports.

## When to Use

- Use this skill when working on tasks related to agent introspection debugging
- Apply best practices from everything-claude-code

## Workflow

name: agent-introspection-debugging
description: Structured self-debugging workflow for AI agent failures using capture, diagnosis, contained recovery, and introspection reports.
origin: ECC
# Agent Introspection Debugging
Use this skill when an agent run is failing repeatedly, consuming tokens without progress, looping on the same tools, or drifting away from the intended task.
This is a workflow skill, not a hidden runtime. It teaches the agent to debug itself systematically before escalating to a human.
## When to Activate
- Maximum tool call / loop-limit failures
- Repeated retries with no

## Source

Adopted from: everything-claude-code
