---
name: 'architecture-decision-records'
description: 'Capture architectural decisions made during Claude Code sessions as structured'
adopted: 2026-05-16
batch: bulk-adoption
ADRs. Auto-detects decision moments, records context, alternatives considered, and
rationale. Maintains an ADR log so fut
source: everything-claude-code
---

# architecture-decision-records

Capture architectural decisions made during Claude Code sessions as structured ADRs. Auto-detects decision moments, records context, alternatives considered, and rationale. Maintains an ADR log so fut

## When to Use

- Use this skill when working on tasks related to architecture decision records
- Apply best practices from everything-claude-code

## Workflow

### Capturing a New ADR

When a decision moment is detected:

1. **Initialize (first time only)** — if `docs/adr/` does not exist, ask the user for confirmation before creating the directory, a `README.md` seeded with the index table header (see ADR Index Format below), and a blank `template.md` for manual use. Do not create files without explicit consent.
2. **Identify the decision** — extract the core architectural choice being made
3. **Gather context** — what problem prompted this? What constraints exist?
4. **Document alternatives** — what other options were considered? Why were they rejected?
5. **State consequences** — what are the trade-offs? What becomes easier/harder?
6. **Assign a number** — scan existing ADRs in `docs/adr/` and increment
7. **Confirm and write** — present the d

## Source

Adopted from: everything-claude-code
