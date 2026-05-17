---
name: 'new-rails-project'
description: 'Create a new Rails project'
adopted: 2026-05-16
batch: bulk-adoption
source: antigravity-awesome-skills
tier: 4
version: 1.0.0
---

# new-rails-project

Create a new Rails project

## When to Use

- Use this skill when working on tasks related to new rails project
- Apply best practices from antigravity-awesome-skills

## Workflow

name: new-rails-project
argument-hint: [project name]
description: Create a new Rails project
allowed-tools: Bash(rails *), Bash(bundle *), Bash(bin/*), Bash(npm *), Bash(yarn *)
context: fork
risk: unknown
source: community
metadata:
  author: Shpigford
  version: "1.0"
Generate a new Rails project named $1 in the current directory. You may reference @CLAUDE.md for general guidance, though the guidance here takes precedence.
## When to Use
- You need to bootstrap a new Rails project with the opinionated stack defined in this skill.
- The project should start with Rails, PostgreSQL, Inertia.js

## Source

Adopted from: antigravity-awesome-skills
