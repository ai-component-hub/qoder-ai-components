---
name: 'autonomous-agent-harness'
description: 'Transform Claude Code into a fully autonomous agent system with persistent'
adopted: 2026-05-16
memory, scheduled operations, computer use, and task queuing. Replaces standalone
agent frameworks (Hermes, AutoGPT) by lever
source: everything-claude-code
tier: 2
---

# autonomous-agent-harness

Transform Claude Code into a fully autonomous agent system with persistent memory, scheduled operations, computer use, and task queuing. Replaces standalone agent frameworks (Hermes, AutoGPT) by lever

## When to Use

- Use this skill when working on tasks related to autonomous agent harness
- Trigger when you need expertise in this domain
- Apply best practices from everything-claude-code

## Workflow

name: autonomous-agent-harness
description: Transform Claude Code into a fully autonomous agent system with persistent memory, scheduled operations, computer use, and task queuing. Replaces standalone agent frameworks (Hermes, AutoGPT) by leveraging Claude Code's native crons, dispatch, MCP tools, and memory. Use when the user wants continuous autonomous operation, scheduled tasks, or a self-directing agent loop.
origin: ECC
# Autonomous Agent Harness
Turn Claude Code into a persistent, self-directing agent system using only native features and MCP servers.
## Consent and Safety Boundaries
Autonomous operation must be explicitly requested and scoped by the user. Do not create schedules, dispatch remote agents, write persistent memory, use computer control, post externally, modify third-party resources, or act on private communications unless the user has approved that capability and the target workspace for the current setup.
Prefer dry-run plans and local queue files before enabling recurring or event-driven actions. Keep credentials, private workspace exports, personal datasets, and account-specific automations out of reusable ECC artifacts.
## When to Activate
- User wants an agent that runs continuously or on a schedule
- Setting up automated workflows that trigger periodically
- Building a personal AI assistant that remembers context across sessions
- User says "run this every day", "check on this regularly", "keep monitoring"
- Wants to replicate functionality from Hermes, AutoGPT, or similar autonomous agent frameworks
- Needs computer use combined with scheduled execution
## Architecture
```
┌──────────────────────────────────────────────────────────────┐
│                    Claude Code Runtime                        │
│                                                              │

## Source

This skill was adopted from open-source repository: everything-claude-code
Original path: autonomous-agent-harness
