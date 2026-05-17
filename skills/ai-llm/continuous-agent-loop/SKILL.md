---
name: 'continuous-agent-loop'
description: 'Patterns for continuous autonomous agent loops with quality gates, evals,'
adopted: 2026-05-16
batch: bulk-adoption
and recovery controls.
source: everything-claude-code
tier: 3
---

# continuous-agent-loop

Patterns for continuous autonomous agent loops with quality gates, evals, and recovery controls.

## When to Use

- Use this skill when working on tasks related to continuous agent loop
- Apply best practices from everything-claude-code

## Workflow

name: continuous-agent-loop
description: Patterns for continuous autonomous agent loops with quality gates, evals, and recovery controls.
origin: ECC
# Continuous Agent Loop
This is the v1.8+ canonical loop skill name. It supersedes `autonomous-loops` while keeping compatibility for one release.
## Loop Selection Flow
```text
Start
  |
  +-- Need strict CI/PR control? -- yes --> continuous-pr
  |
  +-- Need RFC decomposition? -- yes --> rfc-dag
  |
  +-- Need exploratory parallel generation? -- yes --> infinite
  |

## Source

Adopted from: everything-claude-code
