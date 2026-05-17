---
name: 'zeroize-audit'
description: 'Detects missing zeroization of sensitive data in source code and identifies zeroization removed by compiler optimizations, with assembly-level analysis, and control-flow verification. Use for auditin'
version: 1.0.0
source: antigravity-awesome-skills
tier: 4
adopted: 2026-05-16
batch: bulk-adoption
---

# zeroize-audit

"Detects missing zeroization of sensitive data in source code and identifies zeroization removed by compiler optimizations, with assembly-level analysis, and control-flow verification. Use for auditin

## When to Use

- Use this skill when working on tasks related to zeroize audit
- Apply best practices from antigravity-awesome-skills

## Workflow

name: zeroize-audit
description: "Detects missing zeroization of sensitive data in source code and identifies zeroization removed by compiler optimizations, with assembly-level analysis, and control-flow verification. Use for auditing C/C++/Rust code handling secrets, keys, passwords, or other sensitive data."
allowed-tools:
  - Read
  - Grep
  - Glob
  - Bash
  - Write
  - Task
  - AskUserQuestion
  - mcp__serena__activate_project
  - mcp__serena__find_symbol
  - mcp__serena__find_referencing_symbols
  - mcp__serena__get_symbols_overview
risk: unknown

## Source

Adopted from: antigravity-awesome-skills
