---
name: 'power-platform-mcp-connector-suite'
description: 'Generate complete Power Platform custom connector with MCP integration'
adopted: 2026-05-16
for Copilot Studio - includes schema generation, troubleshooting, and validation
source: awesome-copilot
tier: 2
version: 1.0.0
---

# power-platform-mcp-connector-suite

'Generate complete Power Platform custom connector with MCP integration for Copilot Studio - includes schema generation, troubleshooting, and validation'

## When to Use

- Use this skill when working on tasks related to power platform mcp connector suite
- Trigger when you need expertise in this domain
- Apply best practices from awesome-copilot

## Workflow

name: power-platform-mcp-connector-suite
description: 'Generate complete Power Platform custom connector with MCP integration for Copilot Studio - includes schema generation, troubleshooting, and validation'
# Power Platform MCP Connector Suite
Generate comprehensive Power Platform custom connector implementations with Model Context Protocol integration for Microsoft Copilot Studio.
## MCP Capabilities in Copilot Studio
**Currently Supported:**
- ✅ **Tools**: Functions that the LLM can call (with user approval)
- ✅ **Resources**: File-like data that agents can read (must be tool outputs)
**Not Yet Supported:**
- ❌ **Prompts**: Pre-written templates (prepare for future support)
## Connector Generation
Create complete Power Platform connector with:
**Core Files:**
- `apiDefinition.swagger.json` with `x-ms-agentic-protocol: mcp-streamable-1.0`
- `apiProperties.json` with connector metadata and authentication
- `script.csx` with custom C# transformations for MCP JSON-RPC handling
- `readme.md` with connector documentation
**MCP Integration:**
- POST `/mcp` endpoint for JSON-RPC 2.0 communication
- McpResponse and McpErrorResponse schema definitions

## Source

This skill was adopted from open-source repository: awesome-copilot
Original path: power-platform-mcp-connector-suite
