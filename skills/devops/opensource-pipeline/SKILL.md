---
name: 'opensource-pipeline'
description: 'Open-source pipeline: fork, sanitize, and package private projects for safe public release. Chains 3 agents (forker, sanitizer, packager). Triggers:'
version: 1.0.0
source: everything-claude-code
tier: 3
adopted: 2026-05-16
batch: bulk-adoption
---

# opensource-pipeline

"Open-source pipeline: fork, sanitize, and package private projects for safe public release. Chains 3 agents (forker, sanitizer, packager). Triggers: '/opensource', 'open source this', 'make this publ

## When to Use

- Use this skill when working on tasks related to opensource pipeline
- Apply best practices from everything-claude-code

## Workflow

name: opensource-pipeline
description: "Open-source pipeline: fork, sanitize, and package private projects for safe public release. Chains 3 agents (forker, sanitizer, packager). Triggers: '/opensource', 'open source this', 'make this public', 'prepare for open source'."
origin: ECC
# Open-Source Pipeline Skill
Safely open-source any project through a 3-stage pipeline: **Fork** (strip secrets) → **Sanitize** (verify clean) → **Package** (CLAUDE.md + setup.sh + README).
## When to Activate
- User says "open source this project" or "make this public"
- User wants to prepare a private repo for pu

## Source

Adopted from: everything-claude-code
