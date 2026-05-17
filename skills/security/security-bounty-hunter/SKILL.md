---
name: 'security-bounty-hunter'
description: 'Hunt for exploitable, bounty-worthy security issues in repositories.'
adopted: 2026-05-16
batch: bulk-adoption
Focuses on remotely reachable vulnerabilities that qualify for real reports instead
of noisy local-only findings.
source: everything-claude-code
---

# security-bounty-hunter

Hunt for exploitable, bounty-worthy security issues in repositories. Focuses on remotely reachable vulnerabilities that qualify for real reports instead of noisy local-only findings.

## When to Use

- Use this skill when working on tasks related to security bounty hunter
- Apply best practices from everything-claude-code

## Workflow

1. Check scope first: program rules, SECURITY.md, disclosure channel, and exclusions.
2. Find real entrypoints: HTTP handlers, uploads, background jobs, webhooks, parsers, and integration endpoints.
3. Run static tooling where it helps, but treat it as triage input only.
4. Read the real code path end to end.
5. Prove user control reaches a meaningful sink.
6. Confirm exploitability and impact with the smallest safe PoC possible.
7. Check for duplicates before drafting a report.

## Source

Adopted from: everything-claude-code
