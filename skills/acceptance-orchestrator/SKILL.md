---
name: 'acceptance-orchestrator'
description: 'Use when a coding task should be driven end-to-end from issue intake'
adopted: 2026-05-16
batch: bulk-adoption
through implementation, review, deployment, and acceptance verification with minimal
human re-intervention.
source: antigravity-awesome-skills
---

# acceptance-orchestrator

Use when a coding task should be driven end-to-end from issue intake through implementation, review, deployment, and acceptance verification with minimal human re-intervention.

## When to Use

- Use this skill when working on tasks related to acceptance orchestrator
- Apply best practices from antigravity-awesome-skills

## Workflow

1. **Intake**
   - Read issue and extract task goal + DoD.

2. **Issue gate**
   - Use `create-issue-gate` logic.
   - If issue is not `ready` or execution gate is not `allowed`, stop immediately.
   - Do not implement anything while issue remains `draft`.

3. **Execute**
   - Hand off to `closed-loop-delivery` for implementation and local verification.

4. **Review loop**
   - If PR feedback is relevant, batch polling windows as:
     - wait `3m`
     - then `6m`
     - then `10m`
   - After the `10m` round, stop waiting and process all visible comments together.

5. **Deploy and runtime verification**
   - If DoD depends on runtime behavior, deploy only to `dev` by default.
   - Verify with real logs/API/Lambda behavior, not assumptions.

6. **Completion gate**
   - Before any claim of c

## Source

Adopted from: antigravity-awesome-skills
