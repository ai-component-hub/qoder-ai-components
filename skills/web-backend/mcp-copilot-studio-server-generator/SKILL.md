---
name: 'mcp-copilot-studio-server-generator'
description: 'Generate a complete MCP server implementation optimized for Copilot Studio'
adopted: 2026-05-16
batch: bulk-adoption
integration with proper schema constraints and streamable HTTP support
source: awesome-copilot
tier: 3
---

# mcp-copilot-studio-server-generator

'Generate a complete MCP server implementation optimized for Copilot Studio integration with proper schema constraints and streamable HTTP support'

## When to Use

- Use this skill when working on tasks related to mcp copilot studio server generator
- Apply best practices from awesome-copilot

## Workflow

Create a complete MCP server implementation that:

1. **Uses Copilot Studio MCP Pattern:**
   - Implement `x-ms-agentic-protocol: mcp-streamable-1.0`
   - Support JSON-RPC 2.0 communication protocol
   - Provide streamable HTTP endpoint at `/mcp`
   - Follow Power Platform connector structure

2. **Schema Compliance Requirements:**
   - **NO reference types** in tool inputs/outputs (filtered by Copilot Studio)
   - **Single type values only** (not arrays of multiple types)
   - **Avoid enum inputs** (interpreted as string, not enum)
   - Use primitive types: string, number, integer, boolean, array, object
   - Ensure all endpoints return full URIs

3. **MCP Components to Include:**
   - **Tools**: Functions for the language model to call (✅ Supported in Copilot Studio)
   - **Resources**: 

## Source

Adopted from: awesome-copilot
