---
name: 'documentation-lookup'
description: 'Use up-to-date library and framework docs via Context7 MCP instead of'
adopted: 2026-05-16
training data. Activates for setup questions, API references, code examples, or
when the user names a framework (e.g. React, Next.
source: everything-claude-code
tier: 2
---

# documentation-lookup

Use up-to-date library and framework docs via Context7 MCP instead of training data. Activates for setup questions, API references, code examples, or when the user names a framework (e.g. React, Next.

## When to Use

- Use this skill when working on tasks related to documentation lookup
- Trigger when you need expertise in this domain
- Apply best practices from everything-claude-code

## Workflow

name: documentation-lookup
description: Use up-to-date library and framework docs via Context7 MCP instead of training data. Activates for setup questions, API references, code examples, or when the user names a framework (e.g. React, Next.js, Prisma).
origin: ECC
# Documentation Lookup (Context7)
When the user asks about libraries, frameworks, or APIs, fetch current documentation via the Context7 MCP (tools `resolve-library-id` and `query-docs`) instead of relying on training data.
## Core Concepts
- **Context7**: MCP server that exposes live documentation; use it instead of training data for libraries and APIs.
- **resolve-library-id**: Returns Context7-compatible library IDs (e.g. `/vercel/next.js`) from a library name and query.
- **query-docs**: Fetches documentation and code snippets for a given library ID and question. Always call resolve-library-id first to get a valid library ID.
## When to use
Activate when the user:
- Asks setup or configuration questions (e.g. "How do I configure Next.js middleware?")
- Requests code that depends on a library ("Write a Prisma query for...")
- Needs API or reference information ("What are the Supabase auth methods?")
- Mentions specific frameworks or libraries (React, Vue, Svelte, Express, Tailwind, Prisma, Supabase, etc.)
Use this skill whenever the request depends on accurate, up-to-date behavior of a library, framework, or API. Applies across harnesses that have the Context7 MCP configured (e.g. Claude Code, Cursor, Codex).
## How it works
### Step 1: Resolve the Library ID
Call the **resolve-library-id** MCP tool with:
- **libraryName**: The library or product name taken from the user's question (e.g. `Next.js`, `Prisma`, `Supabase`).

## Source

This skill was adopted from open-source repository: everything-claude-code
Original path: documentation-lookup
