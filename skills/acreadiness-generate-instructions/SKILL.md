---
name: 'acreadiness-generate-instructions'
description: 'Generate tailored AI agent instruction files via AgentRC instructions command. Produces .github/copilot-instructions.md (default, recommended for Copilot in VS Code) plus optional per-area .instructi'
version: 1.0.0
source: awesome-copilot
tier: 3
adopted: 2026-05-16
batch: bulk-adoption
---

# acreadiness-generate-instructions

'Generate tailored AI agent instruction files via AgentRC instructions command. Produces .github/copilot-instructions.md (default, recommended for Copilot in VS Code) plus optional per-area .instructi

## When to Use

- Use this skill when working on tasks related to acreadiness generate instructions
- Apply best practices from awesome-copilot

## Workflow

1. **Pick the target file**. **Default to `.github/copilot-instructions.md`.** Switch to `AGENTS.md` only if the user mentions multi-agent / Claude / Cursor support.
2. **Always ask which strategy to use** — `flat` or `nested` — unless the user already specified one in their message or via `--strategy`. Present the trade-off briefly:
   - **Flat** *(default)* — one `.github/copilot-instructions.md`. Simple, easy to review in a single PR. Best for small/medium repos with one stack.
   - **Nested** — hub `.github/copilot-instructions.md` + per-topic `.github/instructions/<topic>.instructions.md` files (each with an `applyTo` glob so VS Code only loads them when relevant). Best for large or multi-stack repos. Add `--claude-md` to also emit `CLAUDE.md`.
   Recommend `nested` proactively when t

## Source

Adopted from: awesome-copilot
