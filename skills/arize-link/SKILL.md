---
name: 'arize-link'
description: 'Generates deep links to the Arize UI for traces, spans, sessions, datasets,'
adopted: 2026-05-16
labeling queues, evaluators, and annotation configs. Produces clickable URLs for
sharing Arize resources with team members.
source: awesome-copilot
tier: 2
---

# arize-link

Generates deep links to the Arize UI for traces, spans, sessions, datasets, labeling queues, evaluators, and annotation configs. Produces clickable URLs for sharing Arize resources with team members. 

## When to Use

- Use this skill when working on tasks related to arize link
- Trigger when you need expertise in this domain
- Apply best practices from awesome-copilot

## Workflow

1. Gather IDs from user, exported data, or URL context.
2. Verify all path IDs are base64-encoded.
3. Determine `startA`/`endA` using the priority order above.
4. Substitute into the appropriate template and present as a clickable markdown link.

## Source

This skill was adopted from open-source repository: awesome-copilot
Original path: arize-link
