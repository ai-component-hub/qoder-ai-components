---
name: 'microsoft-docs'
description: 'Query official Microsoft documentation to find concepts, tutorials, and code examples across Azure, .NET, Agent Framework, Aspire, VS Code, GitHub, and more. Uses Microsoft Learn MCP as the default,'
version: 1.0.0
source: awesome-copilot
tier: 2
adopted: 2026-05-16
---

# microsoft-docs

'Query official Microsoft documentation to find concepts, tutorials, and code examples across Azure, .NET, Agent Framework, Aspire, VS Code, GitHub, and more. Uses Microsoft Learn MCP as the default, 

## When to Use

- Use this skill when working on tasks related to microsoft docs
- Trigger when you need expertise in this domain
- Apply best practices from awesome-copilot

## Workflow

name: microsoft-docs
description: 'Query official Microsoft documentation to find concepts, tutorials, and code examples across Azure, .NET, Agent Framework, Aspire, VS Code, GitHub, and more. Uses Microsoft Learn MCP as the default, with Context7 and Aspire MCP for content that lives outside learn.microsoft.com.'
# Microsoft Docs
Research skill for the Microsoft technology ecosystem. Covers learn.microsoft.com and documentation that lives outside it (VS Code, GitHub, Aspire, Agent Framework repos).
## Default: Microsoft Learn MCP
Use these tools for **everything on learn.microsoft.com** — Azure, .NET, M365, Power Platform, Agent Framework, Semantic Kernel, Windows, and more. This is the primary tool for the vast majority of Microsoft documentation queries.
| Tool | Purpose |
|------|---------|
| `microsoft_docs_search` | Search learn.microsoft.com — concepts, guides, tutorials, configuration |
| `microsoft_code_sample_search` | Find working code snippets from Learn docs. Pass `language` (`python`, `csharp`, etc.) for best results |
| `microsoft_docs_fetch` | Get full page content from a specific URL (when search excerpts aren't enough) |
Use `microsoft_docs_fetch` after search when you need complete tutorials, all config options, or when search excerpts are truncated.
### CLI Alternative
If the Learn MCP server is not available, use the `mslearn` CLI from your terminal or shell (for example, Bash, PowerShell, or cmd) instead:
```bash
# Run directly (no install needed)
npx @microsoft/learn-cli search "BlobClient UploadAsync Azure.Storage.Blobs"
# Or install globally, then run
npm install -g @microsoft/learn-cli
mslearn search "BlobClient UploadAsync Azure.Storage.Blobs"

## Source

This skill was adopted from open-source repository: awesome-copilot
Original path: microsoft-docs
