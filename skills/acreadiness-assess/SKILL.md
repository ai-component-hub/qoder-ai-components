---
name: 'acreadiness-assess'
description: 'Run the AgentRC readiness assessment on the current repository and produce a static HTML dashboard at reports/index.html. Wraps `npx github:microsoft/agentrc readiness` and hands off rendering to the'
version: 1.0.0
source: awesome-copilot
tier: 3
adopted: 2026-05-16
batch: bulk-adoption
---

# acreadiness-assess

'Run the AgentRC readiness assessment on the current repository and produce a static HTML dashboard at reports/index.html. Wraps `npx github:microsoft/agentrc readiness` and hands off rendering to the

## When to Use

- Use this skill when working on tasks related to acreadiness assess
- Apply best practices from awesome-copilot

## Workflow

1. **Confirm prerequisites.** Node 20+ must be on PATH. If unsure, run `node --version`.

2. **Decide on a policy** (optional but encouraged):
   - If the user provided `--policy <source>`, capture it.
   - Otherwise check `agentrc.config.json` for a `policies` array.
   - If neither, run with no policy (built-in defaults).
   - For a primer on policies, suggest the `acreadiness-policy` skill.

3. **Run the readiness scan** in the repo root with structured output:
   ```bash
   npx -y github:microsoft/agentrc readiness --json [--policy <source>] [--per-area]
   ```
   The `CommandResult<T>` JSON envelope is your input for the next step.

4. **Hand off to the `ai-readiness-reporter` custom agent** to interpret the JSON and produce `reports/index.html`. The agent renders via the bundled temp

## Source

Adopted from: awesome-copilot
