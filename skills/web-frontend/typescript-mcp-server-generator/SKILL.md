---
name: 'typescript-mcp-server-generator'
description: 'Generate a complete MCP server project in TypeScript with tools, resources,'
adopted: 2026-05-16
and proper configuration
source: awesome-copilot
tier: 2
version: 1.0.0
---

# typescript-mcp-server-generator

'Generate a complete MCP server project in TypeScript with tools, resources, and proper configuration'

## When to Use

- Use this skill when working on tasks related to typescript mcp server generator
- Trigger when you need expertise in this domain
- Apply best practices from awesome-copilot

## Workflow

name: typescript-mcp-server-generator
description: 'Generate a complete MCP server project in TypeScript with tools, resources, and proper configuration'
# Generate TypeScript MCP Server
Create a complete Model Context Protocol (MCP) server in TypeScript with the following specifications:
## Requirements
1. **Project Structure**: Create a new TypeScript/Node.js project with proper directory structure
2. **NPM Packages**: Include @modelcontextprotocol/sdk, zod@3, and either express (for HTTP) or stdio support
3. **TypeScript Configuration**: Proper tsconfig.json with ES modules support
4. **Server Type**: Choose between HTTP (with Streamable HTTP transport) or stdio-based server
5. **Tools**: Create at least one useful tool with proper schema validation
6. **Error Handling**: Include comprehensive error handling and validation
## Implementation Details
### Project Setup
- Initialize with `npm init` and create package.json
- Install dependencies: `@modelcontextprotocol/sdk`, `zod@3`, and transport-specific packages
- Configure TypeScript with ES modules: `"type": "module"` in package.json
- Add dev dependencies: `tsx` or `ts-node` for development
- Create proper .gitignore file
### Server Configuration
- Use `McpServer` class for high-level implementation

## Source

This skill was adopted from open-source repository: awesome-copilot
Original path: typescript-mcp-server-generator
