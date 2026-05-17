---
name: 'react19-test-patterns'
description: 'Provides before/after patterns for migrating test files to React 19 compatibility,'
adopted: 2026-05-16
batch: bulk-adoption
including act() imports, Simulate removal, and StrictMode call count changes.
source: awesome-copilot
tier: 3
---

# react19-test-patterns

'Provides before/after patterns for migrating test files to React 19 compatibility, including act() imports, Simulate removal, and StrictMode call count changes.'

## When to Use

- Use this skill when working on tasks related to react19 test patterns
- Apply best practices from awesome-copilot

## Workflow

name: react19-test-patterns
description: 'Provides before/after patterns for migrating test files to React 19 compatibility, including act() imports, Simulate removal, and StrictMode call count changes.'
# React 19 Test Migration Patterns
Reference for all test file migrations required by React 19.
## Priority Order
Fix test files in this order; each layer depends on the previous:
1. **`act` import**  fix first, it unblocks everything else
2. **`Simulate` → `fireEvent`**  fix immediately after act
3. **Full react-dom/test-utils cleanup**  remove remaining imports
4. **StrictMode call counts** 

## Source

Adopted from: awesome-copilot
