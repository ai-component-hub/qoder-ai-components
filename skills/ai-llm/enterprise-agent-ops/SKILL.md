---
name: 'enterprise-agent-ops'
description: 'Operate long-lived agent workloads with observability, security boundaries,'
adopted: 2026-05-16
and lifecycle management.
source: everything-claude-code
tier: 2
version: 1.0.0
---

# enterprise-agent-ops

Operate long-lived agent workloads with observability, security boundaries, and lifecycle management.

## When to Use

- Use this skill when working on tasks related to enterprise agent ops
- Trigger when you need expertise in this domain
- Apply best practices from everything-claude-code

## Workflow

name: enterprise-agent-ops
description: Operate long-lived agent workloads with observability, security boundaries, and lifecycle management.
origin: ECC
# Enterprise Agent Ops
Use this skill for cloud-hosted or continuously running agent systems that need operational controls beyond single CLI sessions.
## Operational Domains
1. runtime lifecycle (start, pause, stop, restart)
2. observability (logs, metrics, traces)
3. safety controls (scopes, permissions, kill switches)
4. change management (rollout, rollback, audit)
## Baseline Controls
- immutable deployment artifacts
- least-privilege credentials
- environment-level secret injection
- hard timeout and retry budgets
- audit log for high-risk actions
## Metrics to Track
- success rate
- mean retries per task
- time to recovery

## Source

This skill was adopted from open-source repository: everything-claude-code
Original path: enterprise-agent-ops
