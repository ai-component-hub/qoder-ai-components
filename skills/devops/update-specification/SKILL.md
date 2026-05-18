---
name: 'update-specification'
description: 'Update an existing specification file for the solution, optimized for'
adopted: 2026-05-16
Generative AI consumption based on new requirements or updates to any existing code.
source: awesome-copilot
tier: 2
version: 1.0.0
---

# update-specification

'Update an existing specification file for the solution, optimized for Generative AI consumption based on new requirements or updates to any existing code.'

## When to Use

- Use this skill when working on tasks related to update specification
- Trigger when you need expertise in this domain
- Apply best practices from awesome-copilot

## Workflow

name: update-specification
description: 'Update an existing specification file for the solution, optimized for Generative AI consumption based on new requirements or updates to any existing code.'
# Update Specification
Your goal is to update the existing specification file `${file}` based on new requirements or updates to any existing code.
The specification file must define the requirements, constraints, and interfaces for the solution components in a manner that is clear, unambiguous, and structured for effective use by Generative AIs. Follow established documentation standards and ensure the content is machine-readable and self-contained.
## Best Practices for AI-Ready Specifications
- Use precise, explicit, and unambiguous language.
- Clearly distinguish between requirements, constraints, and recommendations.
- Use structured formatting (headings, lists, tables) for easy parsing.
- Avoid idioms, metaphors, or context-dependent references.
- Define all acronyms and domain-specific terms.
- Include examples and edge cases where applicable.
- Ensure the document is self-contained and does not rely on external context.
The specification should be saved in the [/spec/](/spec/) directory and named according to the following convention: `[a-z0-9-]+.md`, where the name should be descriptive of the specification's content and starting with the highlevel purpose, which is one of [schema, tool, data, infrastructure, process, architecture, or design].
The specification file must be formatted in well formed Markdown.
Specification files must follow the template below, ensuring that all sections are filled out appropriately. The front matter for the markdown should be structured correctly as per the example following:
```md
title: [Concise Title Describing the Specification's Focus]
version: [Optional: e.g., 1.0, Date]
date_created: [YYYY-MM-DD]

## Source

This skill was adopted from open-source repository: awesome-copilot
Original path: update-specification
