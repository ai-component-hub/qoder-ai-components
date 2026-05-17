---
name: 'dashboard-builder'
description: 'Build monitoring dashboards that answer real operator questions for Grafana,'
adopted: 2026-05-16
batch: bulk-adoption
SigNoz, and similar platforms. Use when turning metrics into a working dashboard
instead of a vanity board.
source: everything-claude-code
---

# dashboard-builder

Build monitoring dashboards that answer real operator questions for Grafana, SigNoz, and similar platforms. Use when turning metrics into a working dashboard instead of a vanity board.

## When to Use

- Use this skill when working on tasks related to dashboard builder
- Apply best practices from everything-claude-code

## Workflow

### 1. Define the operating questions

Organize around:

- health / availability
- latency / performance
- throughput / volume
- saturation / resources
- service-specific risk

### 2. Study the target platform schema

Inspect existing dashboards first:

- JSON structure
- query language
- variables
- threshold styling
- section layout

### 3. Build the minimum useful board

Recommended structure:

1. overview
2. performance
3. resources
4. service-specific section

### 4. Cut vanity panels

Every panel should answer a real question. If it does not, remove it.

## Source

Adopted from: everything-claude-code
