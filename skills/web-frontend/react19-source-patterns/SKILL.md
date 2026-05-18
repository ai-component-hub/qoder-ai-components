---
name: 'react19-source-patterns'
description: 'Reference for React 19 source-file migration patterns, including API'
adopted: 2026-05-16
batch: bulk-adoption
changes, ref handling, and context updates.
source: awesome-copilot
tier: 3
---

# react19-source-patterns

'Reference for React 19 source-file migration patterns, including API changes, ref handling, and context updates.'

## When to Use

- Use this skill when working on tasks related to react19 source patterns
- Apply best practices from awesome-copilot

## Workflow

name: react19-source-patterns
description: 'Reference for React 19 source-file migration patterns, including API changes, ref handling, and context updates.'
# React 19 Source Migration Patterns
Reference for every source-file migration required for React 19.
## Quick Reference Table
| Pattern | Action | Reference |
|---|---|---|
| `ReactDOM.render(...)` | → `createRoot().render()` | See references/api-migrations.md |
| `ReactDOM.hydrate(...)` | → `hydrateRoot(...)` | See references/api-migrations.md |
| `unmountComponentAtNode` | → `root.unmount()` | Inline fix |
| `ReactDOM.findDOMNode` | → 

## Source

Adopted from: awesome-copilot
