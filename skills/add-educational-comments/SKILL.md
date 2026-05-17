---
name: 'add-educational-comments'
description: 'Add educational comments to the file specified, or prompt asking for'
adopted: 2026-05-16
file to comment if one is not provided.
source: awesome-copilot
tier: 2
version: 1.0.0
---

# add-educational-comments

'Add educational comments to the file specified, or prompt asking for file to comment if one is not provided.'

## When to Use

- Use this skill when working on tasks related to add educational comments
- Trigger when you need expertise in this domain
- Apply best practices from awesome-copilot

## Workflow

1. **Confirm Inputs** – Ensure at least one target file is provided. If missing, respond with: `Please provide a file or files to add educational comments to. Preferably as chat variable or attached context.`
2. **Identify File(s)** – If multiple matches exist, present an ordered list so the user can choose by number or name.
3. **Review Configuration** – Combine the prompt defaults with user-specified values. Interpret obvious typos (e.g., `Line Numer`) using context.
4. **Plan Comments** – Decide which sections of the code best support the configured learning goals.
5. **Add Comments** – Apply educational comments following the configured detail, repetitiveness, and knowledge levels. Respect indentation and language syntax.
6. **Validate** – Confirm formatting, encoding, and syntax remain intact. Ensure the 125% rule and line limits are satisfied.

## Source

This skill was adopted from open-source repository: awesome-copilot
Original path: add-educational-comments
