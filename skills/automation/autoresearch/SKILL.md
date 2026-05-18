---
name: 'autoresearch'
description: 'Autonomous iterative experimentation loop for any programming task. Guides the user through defining goals, measurable metrics, and scope constraints, then runs an autonomous loop of code changes, te'
version: 1.0.0
source: awesome-copilot
tier: 2
adopted: 2026-05-16
---

# autoresearch

'Autonomous iterative experimentation loop for any programming task. Guides the user through defining goals, measurable metrics, and scope constraints, then runs an autonomous loop of code changes, te

## When to Use

- Use this skill when working on tasks related to autoresearch
- Trigger when you need expertise in this domain
- Apply best practices from awesome-copilot

## Workflow

name: autoresearch
description: 'Autonomous iterative experimentation loop for any programming task. Guides the user through defining goals, measurable metrics, and scope constraints, then runs an autonomous loop of code changes, testing, measuring, and keeping/discarding results. Inspired by Karpathy''s autoresearch. USE FOR: autonomous improvement, iterative optimization, experiment loop, auto research, performance tuning, automated experimentation, hill climbing, try things automatically, optimize code, run experiments, autonomous coding loop. DO NOT USE FOR: one-shot tasks, simple bug fixes, code review, or tasks without a measurable metric.'
license: MIT
compatibility: Requires git. The project must be a git repository. Requires terminal access to run commands.
metadata:
  author: luiscantero
  inspired-by: https://github.com/karpathy/autoresearch
# Autoresearch: Autonomous Iterative Experimentation
An autonomous experimentation loop for any programming task. You define the goal and how to measure it; the agent iterates autonomously -- modifying code, running experiments, measuring results, and keeping or discarding changes -- until interrupted.
This skill is inspired by [Karpathy's autoresearch](https://github.com/karpathy/autoresearch), generalized from ML training to **any programming task with a measurable outcome**.
## Agent Behavior Rules
1. **DO** guide the user through the Setup phase interactively before starting the loop.
2. **DO** establish a baseline measurement before making any changes.
3. **DO** commit every experiment attempt before running it (so it can be reverted cleanly).
4. **DO** keep a results log (TSV) tracking every experiment.
5. **DO** revert changes that do not improve the metric (git reset to last known good).
6. **DO** run autonomously once the loop starts -- never pause to ask "should I continue?".
7. **DO NOT** modify files the user marked as out-of-scope.
8. **DO NOT** skip the measurement step -- every experiment must be measured.
9. **DO NOT** keep changes that regress the metric unless the user explicitly allowed trade-offs.

## Source

This skill was adopted from open-source repository: awesome-copilot
Original path: autoresearch
