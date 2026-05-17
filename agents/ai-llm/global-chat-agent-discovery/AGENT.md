---
name: 'global-chat-agent-discovery'
description: 'Discover and search 18K+ MCP servers and AI agents across 6+ registries'
using Global Chat's cross-protocol directory and MCP server.
source: open-source (antigravity-awesome-skills)
type: autonomous_agent_skill
version: 1.0
---

# Global Chat Agent Discovery

"Discover and search 18K+ MCP servers and AI agents across 6+ registries using Global Chat's cross-protocol directory and MCP server."

## Autonomous Capabilities

- Autonomous operation without manual intervention
- Intelligent task planning and execution
- Self-monitoring and error recovery
- Multi-step workflow orchestration

## Use Cases

- Automated task execution
- Complex workflow management
- Intelligent decision making
- Autonomous problem solving

## Workflow

1. Initialize agent with task parameters
2. Analyze task requirements
3. Execute autonomous workflow
4. Monitor progress and handle errors
5. Report results and completion status

## Source

This autonomous agent was adopted from: `antigravity-awesome-skills/skills/global-chat-agent-discovery/SKILL.md`

## Original Content

---
name: global-chat-agent-discovery
description: "Discover and search 18K+ MCP servers and AI agents across 6+ registries using Global Chat's cross-protocol directory and MCP server."
category: development
risk: safe
source: community
source_repo: pumanitro/global-chat
source_type: community
date_added: "2026-04-06"
author: pumanitro
tags: [mcp, ai-agents, agent-discovery, agents-txt, a2a, developer-tools]
tools: [claude, cursor, gemini, codex]
---

# Global Chat Agent Discovery

## Overview

Global Chat is a cross-protocol AI agent discovery platform that aggregates MCP servers and AI agents from 6+ registries into a single searchable directory. This skill helps you find the right MCP server, A2A agent, or agents.txt endpoint for any task by searching across 18,000+ indexed entries. It also provides an MCP server (`@global-chat/mcp-server`) for programmatic access to the directory from any MCP-compatible client.

## When to Use This Skill

- Use when you need to find an MCP server for a specific capability (e.g., database access, file conversion, API integration)
- Use when evaluating which agent registries carry tools for your use case
- Use when you want to search across multiple protocols (MCP, A2A, agents.txt) simultaneously
- Use when setting up agent-to-agent communication and need to discover available endpoints

## How It Works

### Option 1: Use the MCP Server (Recommended for Agents)

Install the Global Chat MCP server to search the directory programmatically from Claude Code, Cursor, or any MCP client.

```bash
npm install -g @global-chat/mcp-server
```

Add to your MCP client configuration:

```json
{
  "mcpServers": {
    "global-chat": {
      "command": "npx",
      "args": ["-y", "@global-chat/mcp-server"]
    }
  }
}
```

Then ask your agent to search for tools:

```
Search Global Chat for MCP servers that handle PostgreSQL database queries.
```

### Option 2: Use the Web Directory

Browse the full directory at [https://global-chat.io](https://gl
