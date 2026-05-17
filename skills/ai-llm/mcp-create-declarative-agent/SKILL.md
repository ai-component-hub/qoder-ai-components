---
name: 'mcp-create-declarative-agent'
description: 'Skill converted from mcp-create-declarative-agent.prompt.md'
adopted: 2026-05-16
source: awesome-copilot
tier: 2
version: 1.0.0
---

# mcp-create-declarative-agent

'Skill converted from mcp-create-declarative-agent.prompt.md'

## When to Use

- Use this skill when working on tasks related to mcp create declarative agent
- Trigger when you need expertise in this domain
- Apply best practices from awesome-copilot

## Workflow

Ask the user:
1. What MCP server are you integrating with (URL)?
2. What tools should be exposed to Copilot?
3. What authentication method does the server support?
4. What should the agent's primary purpose be?
5. Do you need response semantics or Adaptive Cards?

Then generate:
- Complete appPackage/ structure (manifest.json, declarativeAgent.json, ai-plugin.json)
- mcp.json configuration
- .env.local template
- Provisioning and testing instructions

## Source

This skill was adopted from open-source repository: awesome-copilot
Original path: mcp-create-declarative-agent
