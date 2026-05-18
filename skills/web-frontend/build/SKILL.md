---
name: 'build'
description: 'build'
adopted: 2026-05-16
batch: bulk-adoption
source: antigravity-awesome-skills
tier: 4
version: 1.0.0
---

# build

build

## When to Use

- Use this skill when working on tasks related to build
- Apply best practices from antigravity-awesome-skills

## Workflow

This command manages a 4-phase feature development workflow for building major features. Parse `$ARGUMENTS` to determine which subcommand to run.

**Arguments provided:** $ARGUMENTS

### Argument Parsing

Parse the first word of $ARGUMENTS to determine the subcommand:

- `research [name]` → Run the Research phase
- `implementation [name]` → Run the Implementation phase
- `progress [name]` → Run the Progress phase
- `phase [n] [name]` → Run Phase n of the implementation
- `status [name]` → Show current status and suggest next step
- (empty or unrecognized) → Show usage help

If the feature name is not provided in arguments, you MUST use AskUserQuestion to prompt for it.

---

## Source

Adopted from: antigravity-awesome-skills
