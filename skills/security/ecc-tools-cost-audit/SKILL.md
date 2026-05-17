---
name: 'ecc-tools-cost-audit'
description: 'Evidence-first ECC Tools burn and billing audit workflow. Use when investigating'
adopted: 2026-05-16
batch: bulk-adoption
runaway PR creation, quota bypass, premium-model leakage, duplicate jobs, or GitHub
App cost spikes in the ECC Tools re
source: everything-claude-code
---

# ecc-tools-cost-audit

Evidence-first ECC Tools burn and billing audit workflow. Use when investigating runaway PR creation, quota bypass, premium-model leakage, duplicate jobs, or GitHub App cost spikes in the ECC Tools re

## When to Use

- Use this skill when working on tasks related to ecc tools cost audit
- Apply best practices from everything-claude-code

## Workflow

### 1. Freeze repo scope

- switch into the sibling `ECC-Tools` repo
- check branch and local diff first
- identify the exact surface under audit:
  - webhook router
  - queue producer
  - queue consumer
  - PR creation path
  - usage reservation / billing path
  - model routing path

### 2. Trace ingress before theorizing

- inspect `src/index.*` or the main entrypoint first
- map every enqueue path before suggesting a fix
- confirm which GitHub events share a queue type
- confirm whether push, pull_request, synchronize, comment, or manual re-run events can converge on the same expensive path

### 3. Trace the worker and side effects

- inspect the queue consumer or scheduled worker that handles analysis
- confirm whether a queued analysis always ends in:
  - PR creation
  - branch creati

## Source

Adopted from: everything-claude-code
