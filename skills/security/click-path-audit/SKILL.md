---
name: 'click-path-audit'
description: 'Trace every user-facing button/touchpoint through its full state change sequence to find bugs where functions individually work but cancel each other out, produce wrong final state, or leave the UI i'
version: 1.0.0
source: everything-claude-code
tier: 2
adopted: 2026-05-16
---

# click-path-audit

"Trace every user-facing button/touchpoint through its full state change sequence to find bugs where functions individually work but cancel each other out, produce wrong final state, or leave the UI i

## When to Use

- Use this skill when working on tasks related to click path audit
- Trigger when you need expertise in this domain
- Apply best practices from everything-claude-code

## Workflow

name: click-path-audit
description: "Trace every user-facing button/touchpoint through its full state change sequence to find bugs where functions individually work but cancel each other out, produce wrong final state, or leave the UI in an inconsistent state. Use when: systematic debugging found no bugs but users report broken buttons, or after any major refactor touching shared state stores."
origin: community
# /click-path-audit — Behavioural Flow Audit
Find bugs that static code reading misses: state interaction side effects, race conditions between sequential calls, and handlers that silently undo each other.
## The Problem This Solves
Traditional debugging checks:
- Does the function exist? (missing wiring)
- Does it crash? (runtime errors)
- Does it return the right type? (data flow)
But it does NOT check:
- **Does the final UI state match what the button label promises?**
- **Does function B silently undo what function A just did?**
- **Does shared state (Zustand/Redux/context) have side effects that cancel the intended action?**
Real example: A "New Email" button called `setComposeMode(true)` then `selectThread(null)`. Both worked individually. But `selectThread` had a side effect resetting `composeMode: false`. The button did nothing. 54 bugs were found by systematic debugging — this one was missed.
## How It Works
For EVERY interactive touchpoint in the target area:
```
1. IDENTIFY the handler (onClick, onSubmit, onChange, etc.)
2. TRACE every function call in the handler, IN ORDER

## Source

This skill was adopted from open-source repository: everything-claude-code
Original path: click-path-audit
