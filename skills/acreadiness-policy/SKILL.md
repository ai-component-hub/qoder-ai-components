---
name: 'acreadiness-policy'
description: 'Help the user pick, write, or apply an AgentRC policy. Policies customise readiness scoring by disabling irrelevant checks, overriding impact/level, setting pass-rate thresholds, or chaining org base'
version: 1.0.0
source: awesome-copilot
tier: 2
adopted: 2026-05-16
---

# acreadiness-policy

'Help the user pick, write, or apply an AgentRC policy. Policies customise readiness scoring by disabling irrelevant checks, overriding impact/level, setting pass-rate thresholds, or chaining org base

## When to Use

- Use this skill when working on tasks related to acreadiness policy
- Trigger when you need expertise in this domain
- Apply best practices from awesome-copilot

## Workflow

name: acreadiness-policy
description: 'Help the user pick, write, or apply an AgentRC policy. Policies customise readiness scoring by disabling irrelevant checks, overriding impact/level, setting pass-rate thresholds, or chaining org baselines with team overrides. Use when the user asks about strict mode, AI-only scoring, custom weights, CI gating, or wants org-wide standardisation.'
argument-hint: "[show | new <name> | apply <path-or-pkg>] — e.g. /acreadiness-policy show, /acreadiness-policy new strict-frontend"
# /acreadiness-policy — AgentRC policies
Use this skill when the user asks about **policies**, **strict mode**, **custom scoring**, **disabling checks**, **org standards**, or **CI gating** of readiness.
A policy is a small JSON file with three optional sections — `criteria`, `extras`, `thresholds` — that customise how AgentRC scores readiness.
## Built-in examples
AgentRC ships with three example policies in `examples/policies/`:
| Policy | What it does |
|---|---|
| `strict.json` | 100% pass rate, raises impact on key criteria |
| `ai-only.json` | Disables all repo-health checks, focuses on AI tooling |
| `repo-health-only.json` | Disables AI checks, focuses on traditional quality |
Recommend these as starting points before writing a custom policy.
## Policy schema
```jsonc
{
  "name": "my-policy",
  "criteria": {
    "disable":  ["env-example", "observability", "dependabot"],

## Source

This skill was adopted from open-source repository: awesome-copilot
Original path: acreadiness-policy
