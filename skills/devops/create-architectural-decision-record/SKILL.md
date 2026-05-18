---
name: 'create-architectural-decision-record'
description: 'Create an Architectural Decision Record (ADR) document for AI-optimized'
adopted: 2026-05-16
decision documentation.
source: awesome-copilot
tier: 2
version: 1.0.0
---

# create-architectural-decision-record

'Create an Architectural Decision Record (ADR) document for AI-optimized decision documentation.'

## When to Use

- Use this skill when working on tasks related to create architectural decision record
- Trigger when you need expertise in this domain
- Apply best practices from awesome-copilot

## Workflow

name: create-architectural-decision-record
description: 'Create an Architectural Decision Record (ADR) document for AI-optimized decision documentation.'
# Create Architectural Decision Record
Create an ADR document for `${input:DecisionTitle}` using structured formatting optimized for AI consumption and human readability.
## Inputs
- **Context**: `${input:Context}`
- **Decision**: `${input:Decision}`
- **Alternatives**: `${input:Alternatives}`
- **Stakeholders**: `${input:Stakeholders}`
## Input Validation
If any of the required inputs are not provided or cannot be determined from the conversation history, ask the user to provide the missing information before proceeding with ADR generation.
## Requirements
- Use precise, unambiguous language
- Follow standardized ADR format with front matter
- Include both positive and negative consequences
- Document alternatives with rejection rationale
- Structure for machine parsing and human reference
- Use coded bullet points (3-4 letter codes + 3-digit numbers) for multi-item sections
The ADR must be saved in the `/docs/adr/` directory using the naming convention: `adr-NNNN-[title-slug].md`, where NNNN is the next sequential 4-digit number (e.g., `adr-0001-database-selection.md`).
## Required Documentation Structure

## Source

This skill was adopted from open-source repository: awesome-copilot
Original path: create-architectural-decision-record
