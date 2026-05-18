---
name: 'social-graph-ranker'
description: 'Weighted social-graph ranking for warm intro discovery, bridge scoring,'
adopted: 2026-05-16
batch: bulk-adoption
and network gap analysis across X and LinkedIn. Use when the user wants the reusable
graph-ranking engine itself, not the broade
source: everything-claude-code
---

# social-graph-ranker

Weighted social-graph ranking for warm intro discovery, bridge scoring, and network gap analysis across X and LinkedIn. Use when the user wants the reusable graph-ranking engine itself, not the broade

## When to Use

- Use this skill when working on tasks related to social graph ranker
- Apply best practices from everything-claude-code

## Workflow

1. Build the weighted target set.
2. Pull the user's graph from X, LinkedIn, or both.
3. Compute direct bridge scores.
4. Expand second-order candidates for the highest-value mutuals.
5. Rank by `R(m)`.
6. Return:
   - best warm intro asks
   - conditional bridge paths
   - graph gaps where no warm path exists

## Source

Adopted from: everything-claude-code
