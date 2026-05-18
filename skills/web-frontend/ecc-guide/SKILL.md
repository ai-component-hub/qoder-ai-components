---
name: 'ecc-guide'
description: 'Guide users through ECC'
adopted: 2026-05-16
install profiles, and project onboarding by reading the live repository surface
before answering.
source: everything-claude-code
tier: 2
---

# ecc-guide

Guide users through ECC's current agents, skills, commands, hooks, rules, install profiles, and project onboarding by reading the live repository surface before answering.

## When to Use

- Use this skill when working on tasks related to ecc guide
- Trigger when you need expertise in this domain
- Apply best practices from everything-claude-code

## Workflow

name: ecc-guide
description: Guide users through ECC's current agents, skills, commands, hooks, rules, install profiles, and project onboarding by reading the live repository surface before answering.
origin: community
# ECC Guide
Use this skill when a user needs help understanding, navigating, installing, or choosing parts of Everything Claude Code.
## When To Use
Use this skill when the user:
- asks what ECC includes
- wants help finding a skill, command, agent, hook, rule, or install profile
- is new to the repository and needs a guided path
- asks "how do I do X with ECC?"
- asks which ECC components fit a project
- needs a lightweight explanation of how commands, skills, agents, hooks, and rules relate
- is confused by install paths, duplicate installs, reset/uninstall, or selective install options
## Core Principle
Answer from current files, not memory. ECC changes quickly, so hard-coded catalog counts, feature lists, and install instructions go stale.
When the ECC repository is available, inspect the relevant files before giving a concrete answer:
```bash
node scripts/ci/catalog.js --json
find skills -maxdepth 2 -name SKILL.md | sort

## Source

This skill was adopted from open-source repository: everything-claude-code
Original path: ecc-guide
