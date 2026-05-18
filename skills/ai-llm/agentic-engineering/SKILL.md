---
name: 'agentic-engineering'
description: 'Operate as an agentic engineer using eval-first execution, decomposition,'
adopted: 2026-05-16
and cost-aware model routing.
source: everything-claude-code
tier: 2
version: 1.0.0
---

# agentic-engineering

Operate as an agentic engineer using eval-first execution, decomposition, and cost-aware model routing.

## When to Use

- Use this skill when working on tasks related to agentic engineering
- Trigger when you need expertise in this domain
- Apply best practices from everything-claude-code

## Workflow

name: agentic-engineering
description: Operate as an agentic engineer using eval-first execution, decomposition, and cost-aware model routing.
origin: ECC
# Agentic Engineering
Use this skill for engineering workflows where AI agents perform most implementation work and humans enforce quality and risk controls.
## Operating Principles
1. Define completion criteria before execution.
2. Decompose work into agent-sized units.
3. Route model tiers by task complexity.
4. Measure with evals and regression checks.
## Eval-First Loop
1. Define capability eval and regression eval.
2. Run baseline and capture failure signatures.
3. Execute implementation.
4. Re-run evals and compare deltas.
## Task Decomposition
Apply the 15-minute unit rule:
- each unit should be independently verifiable
- each unit should have a single dominant risk
- each unit should expose a clear done condition

## Source

This skill was adopted from open-source repository: everything-claude-code
Original path: agentic-engineering
