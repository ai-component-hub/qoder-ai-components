---
name: 'security-scan'
description: 'Scan your Claude Code configuration (.claude/ directory) for security'
adopted: 2026-05-16
vulnerabilities, misconfigurations, and injection risks using AgentShield. Checks
CLAUDE.md, settings.json, MCP servers, hooks, an
source: everything-claude-code
tier: 2
---

# security-scan

Scan your Claude Code configuration (.claude/ directory) for security vulnerabilities, misconfigurations, and injection risks using AgentShield. Checks CLAUDE.md, settings.json, MCP servers, hooks, an

## When to Use

- Use this skill when working on tasks related to security scan
- Trigger when you need expertise in this domain
- Apply best practices from everything-claude-code

## Workflow

name: security-scan
description: Scan your Claude Code configuration (.claude/ directory) for security vulnerabilities, misconfigurations, and injection risks using AgentShield. Checks CLAUDE.md, settings.json, MCP servers, hooks, and agent definitions.
origin: ECC
# Security Scan Skill
Audit your Claude Code configuration for security issues using [AgentShield](https://github.com/affaan-m/agentshield).
## When to Activate
- Setting up a new Claude Code project
- After modifying `.claude/settings.json`, `CLAUDE.md`, or MCP configs
- Before committing configuration changes
- When onboarding to a new repository with existing Claude Code configs
- Periodic security hygiene checks
## What It Scans
| File | Checks |
|------|--------|
| `CLAUDE.md` | Hardcoded secrets, auto-run instructions, prompt injection patterns |
| `settings.json` | Overly permissive allow lists, missing deny lists, dangerous bypass flags |
| `mcp.json` | Risky MCP servers, hardcoded env secrets, npx supply chain risks |
| `hooks/` | Command injection via interpolation, data exfiltration, silent error suppression |
| `agents/*.md` | Unrestricted tool access, prompt injection surface, missing model specs |
## Prerequisites

## Source

This skill was adopted from open-source repository: everything-claude-code
Original path: security-scan
