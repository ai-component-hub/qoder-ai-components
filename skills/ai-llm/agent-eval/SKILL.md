---
name: 'agent-eval'
description: 'Head-to-head comparison of coding agents (Claude Code, Aider, Codex,'
adopted: 2026-05-16
etc.) on custom tasks with pass rate, cost, time, and consistency metrics
source: everything-claude-code
tier: 2
version: 1.0.0
---

# agent-eval

Head-to-head comparison of coding agents (Claude Code, Aider, Codex, etc.) on custom tasks with pass rate, cost, time, and consistency metrics

## When to Use

- Use this skill when working on tasks related to agent eval
- Trigger when you need expertise in this domain
- Apply best practices from everything-claude-code

## Workflow

### 1. Define Tasks

Create a `tasks/` directory with YAML files, one per task:

```bash
mkdir tasks
# Write task definitions (see template above)
```

### 2. Run Agents

Execute agents against your tasks:

```bash
agent-eval run --task tasks/add-retry-logic.yaml --agent claude-code --agent aider --runs 3
```

Each run:
1. Creates a fresh git worktree from the specified commit
2. Hands the prompt to the agent
3. Runs the judge criteria
4. Records pass/fail, cost, and time

### 3. Compare Results

Generate a comparison report:

```bash
agent-eval report --format table
```

```
Task: add-retry-logic (3 runs each)
┌──────────────┬───────────┬────────┬────────┬─────────────┐
│ Agent        │ Pass Rate │ Cost   │ Time   │ Consistency │
├──────────────┼───────────┼────────┼────────┼─────────────┤
│ claude-code  │ 3/3       │ $0.12  │ 45s    │ 100%        │
│ aider        │ 2/3       │ $0.08  │ 38s    │  67%        │
└──────────────┴───────────┴────────┴────────┴─────────────┘
```

## Source

This skill was adopted from open-source repository: everything-claude-code
Original path: agent-eval
