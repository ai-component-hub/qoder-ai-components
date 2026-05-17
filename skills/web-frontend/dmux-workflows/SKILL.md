---
name: 'dmux-workflows'
description: 'Multi-agent orchestration using dmux (tmux pane manager for AI agents).'
adopted: 2026-05-16
Patterns for parallel agent workflows across Claude Code, Codex, OpenCode, and other
harnesses. Use when running multiple agent
source: everything-claude-code
tier: 2
---

# dmux-workflows

Multi-agent orchestration using dmux (tmux pane manager for AI agents). Patterns for parallel agent workflows across Claude Code, Codex, OpenCode, and other harnesses. Use when running multiple agent 

## When to Use

- Use this skill when working on tasks related to dmux workflows
- Trigger when you need expertise in this domain
- Apply best practices from everything-claude-code

## Workflow

name: dmux-workflows
description: Multi-agent orchestration using dmux (tmux pane manager for AI agents). Patterns for parallel agent workflows across Claude Code, Codex, OpenCode, and other harnesses. Use when running multiple agent sessions in parallel or coordinating multi-agent development workflows.
origin: ECC
# dmux Workflows
Orchestrate parallel AI agent sessions using dmux, a tmux pane manager for agent harnesses.
## When to Activate
- Running multiple agent sessions in parallel
- Coordinating work across Claude Code, Codex, and other harnesses
- Complex tasks that benefit from divide-and-conquer parallelism
- User says "run in parallel", "split this work", "use dmux", or "multi-agent"
## What is dmux
dmux is a tmux-based orchestration tool that manages AI agent panes:
- Press `n` to create a new pane with a prompt
- Press `m` to merge pane output back to the main session
- Supports: Claude Code, Codex, OpenCode, Cline, Gemini, Qwen
**Install:** Install dmux from its repository after reviewing the package. See [github.com/standardagents/dmux](https://github.com/standardagents/dmux)
## Quick Start
```bash
# Start dmux session
dmux

## Source

This skill was adopted from open-source repository: everything-claude-code
Original path: dmux-workflows
