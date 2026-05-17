---
name: 'project-skill-audit'
description: 'Audit a project and recommend the highest-value skills to add or update.'
adopted: 2026-05-16
batch: bulk-adoption
source: antigravity-awesome-skills
tier: 4
version: 1.0.0
---

# project-skill-audit

Audit a project and recommend the highest-value skills to add or update.

## When to Use

- Use this skill when working on tasks related to project skill audit
- Apply best practices from antigravity-awesome-skills

## Workflow

1. Map the current project surface.
   Identify the repo root and read the most relevant project guidance first, such as `AGENTS.md`, `README.md`, roadmap/ledger files, and local docs that define workflows or validation expectations.

2. Build the memory/session path first.
   Resolve the memory base as `$CODEX_HOME` when set, otherwise default to `~/.codex`.
   Use these locations:
   - memory index: `$CODEX_HOME/memories/MEMORY.md` or `~/.codex/memories/MEMORY.md`
   - rollout summaries: `$CODEX_HOME/memories/rollout_summaries/`
   - raw sessions: `$CODEX_HOME/sessions/` or `~/.codex/sessions/`

3. Read project past sessions in this order.
   If the runtime prompt already includes a memory summary, start there.
   Then search `MEMORY.md` for:
   - repo name
   - repo basename
   - curren

## Source

Adopted from: antigravity-awesome-skills
