---
name: 'finance-billing-ops'
description: 'Evidence-first revenue, pricing, refunds, team-billing, and billing-model'
adopted: 2026-05-16
truth workflow for ECC. Use when the user wants a sales snapshot, pricing comparison,
duplicate-charge diagnosis, or code-back
source: everything-claude-code
tier: 2
---

# finance-billing-ops

Evidence-first revenue, pricing, refunds, team-billing, and billing-model truth workflow for ECC. Use when the user wants a sales snapshot, pricing comparison, duplicate-charge diagnosis, or code-back

## When to Use

- Use this skill when working on tasks related to finance billing ops
- Trigger when you need expertise in this domain
- Apply best practices from everything-claude-code

## Workflow

### 1. Start from the freshest billing evidence

Prefer live billing data. If the data is not live, state the snapshot timestamp explicitly.

Normalize the picture:

- paid sales
- active subscriptions
- failed or incomplete checkouts
- refunds
- disputes
- duplicate subscriptions

### 2. Separate customer incidents from product truth

If the question is customer-specific, classify first:

- duplicate checkout
- real team intent
- broken self-serve controls
- unmet product value
- failed payment or incomplete setup

Then separate that from the broader product question:

- does team billing really exist?
- are seats actually counted?
- does checkout quantity change entitlement?
- does the site overstate current behavior?

### 3. Inspect code-backed billing behavior

If the answer depends on implementation truth, inspect the code path:

- checkout
- pricing page
- entitlement calculation
- seat or quota handling
- installation vs user usage logic
- billing portal or self-serve management support

### 4. End with a decision and product gap

Report:

- sales snapshot
- issue diagnosis
- product truth
- recommended operator action
- product or backlog gap

## Source

This skill was adopted from open-source repository: everything-claude-code
Original path: finance-billing-ops
