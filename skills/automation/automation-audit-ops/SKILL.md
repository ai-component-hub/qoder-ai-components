---
name: 'automation-audit-ops'
description: 'Evidence-first automation inventory and overlap audit workflow for ECC.'
adopted: 2026-05-16
Use when the user wants to know which jobs, hooks, connectors, MCP servers, or wrappers
are live, broken, redundant, or missing
source: everything-claude-code
tier: 2
---

# automation-audit-ops

Evidence-first automation inventory and overlap audit workflow for ECC. Use when the user wants to know which jobs, hooks, connectors, MCP servers, or wrappers are live, broken, redundant, or missing 

## When to Use

- Use this skill when working on tasks related to automation audit ops
- Trigger when you need expertise in this domain
- Apply best practices from everything-claude-code

## Workflow

### 1. Inventory the real surface

Read the current live surface before theorizing:

- repo hooks and local hook scripts
- GitHub Actions and scheduled workflows
- MCP configs and enabled servers
- connector- or app-backed integrations
- wrapper scripts and repo-specific automation entrypoints

Group them by surface:

- local runtime
- repo CI / automation
- connected external systems
- messaging / notifications
- billing / customer operations
- research / monitoring

### 2. Classify each item by live state

For every surfaced automation, mark:

- configured
- authenticated
- recently verified
- stale or broken
- missing

Then classify the problem type:

- active breakage
- auth outage
- stale status
- overlap or redundancy
- missing capability

### 3. Trace the proof path

Back every important claim with a concrete source:

- file path
- workflow run
- hook log
- config entry
- recent command output
- exact failure signature

If the current state is ambiguous, say so directly instead of pretending the audit is complete.

### 4. End with keep / merge / cut / fix-next

For each overlapping or suspect surface, return one call:

- keep
- merge
- cut
- fix next

The value is in collapsing noisy automation into one canonical ECC lane, not in preserving every historical path.

## Source

This skill was adopted from open-source repository: everything-claude-code
Original path: automation-audit-ops
