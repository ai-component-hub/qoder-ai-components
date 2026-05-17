---
name: 'tldr-prompt'
description: 'Create tldr summaries for GitHub Copilot files (prompts, agents, instructions,'
adopted: 2026-05-16
batch: bulk-adoption
collections), MCP servers, or documentation from URLs and queries.
source: awesome-copilot
tier: 3
---

# tldr-prompt

'Create tldr summaries for GitHub Copilot files (prompts, agents, instructions, collections), MCP servers, or documentation from URLs and queries.'

## When to Use

- Use this skill when working on tasks related to tldr prompt
- Apply best practices from awesome-copilot

## Workflow

You MUST follow these steps in order:

1. **Validate Input**: Confirm at least one required parameter is provided. If not, output the error
message from Error Handling section
2. **Identify Context**:
   - Determine file type (.prompt.md, .agent.md, .instructions.md, .collections.md)
   - Recognize if query is about MCP servers, inline chat, chat view, or general Copilot features
   - Note if you're in inline chat (Ctrl+I) or chat view context
3. **Fetch Content**:
   - For files: Read the file(s) using available file tools
   - For URLs: Fetch content using `#tool:fetch`
   - For queries: Apply URL Resolver strategy to find and fetch relevant content
4. **Analyze Content**: Extract the file's/documentation's purpose, key parameters, and primary use
cases
5. **Generate tldr**: Create summa

## Source

Adopted from: awesome-copilot
