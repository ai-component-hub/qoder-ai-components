---
name: 'aspire'
description: 'Aspire skill covering the Aspire CLI, AppHost orchestration, service discovery, integrations, MCP server, VS Code extension, Dev Containers, GitHub Codespaces, templates, dashboard, and deployment. U'
version: 1.0.0
source: awesome-copilot
tier: 2
adopted: 2026-05-16
---

# aspire

'Aspire skill covering the Aspire CLI, AppHost orchestration, service discovery, integrations, MCP server, VS Code extension, Dev Containers, GitHub Codespaces, templates, dashboard, and deployment. U

## When to Use

- Use this skill when working on tasks related to aspire
- Trigger when you need expertise in this domain
- Apply best practices from awesome-copilot

## Workflow

name: aspire
description: 'Aspire skill covering the Aspire CLI, AppHost orchestration, service discovery, integrations, MCP server, VS Code extension, Dev Containers, GitHub Codespaces, templates, dashboard, and deployment. Use when the user asks to create, run, debug, configure, deploy, or troubleshoot an Aspire distributed application.'
# Aspire — Polyglot Distributed-App Orchestration
Aspire is a **code-first, polyglot toolchain** for building observable, production-ready distributed applications. It orchestrates containers, executables, and cloud resources from a single AppHost project — regardless of whether the workloads are C#, Python, JavaScript/TypeScript, Go, Java, Rust, Bun, Deno, or PowerShell.
> **Mental model:** The AppHost is a *conductor* — it doesn't play the instruments, it tells every service when to start, how to find each other, and watches for problems.
Detailed reference material lives in the `references/` folder — load on demand.
## References
| Reference | When to load |
|---|---|
| [CLI Reference](references/cli-reference.md) | Command flags, options, or detailed usage |
| [MCP Server](references/mcp-server.md) | Setting up MCP for AI assistants, available tools |
| [Integrations Catalog](references/integrations-catalog.md) | Discovering integrations via MCP tools, wiring patterns |
| [Polyglot APIs](references/polyglot-apis.md) | Method signatures, chaining options, language-specific patterns |
| [Architecture](references/architecture.md) | DCP internals, resource model, service discovery, networking, telemetry |
| [Dashboard](references/dashboard.md) | Dashboard features, standalone mode, GenAI Visualizer |
| [Deployment](references/deployment.md) | Docker, Kubernetes, Azure Container Apps, App Service |
| [Testing](references/testing.md) | Integration tests against the AppHost |
| [Troubleshooting](references/troubleshooting.md) | Diagnostic codes, common errors, and fixes |
## 1. Researching Aspire Documentation
The Aspire team ships an **MCP server** that provides documentation tools directly inside your AI assistant. See [MCP Server](references/mcp-server.md) for setup details.

## Source

This skill was adopted from open-source repository: awesome-copilot
Original path: aspire
