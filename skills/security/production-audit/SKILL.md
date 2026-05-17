---
name: 'production-audit'
description: 'Audit a shipped repo for production-readiness gaps across RLS, webhooks,'
adopted: 2026-05-16
secrets, grants, Stripe idempotency, mobile UX, and deployment health.
source: antigravity-awesome-skills
tier: 2
version: 1.0.0
---

# production-audit

"Audit a shipped repo for production-readiness gaps across RLS, webhooks, secrets, grants, Stripe idempotency, mobile UX, and deployment health."

## When to Use

- Use this skill when working on tasks related to production audit
- Trigger when you need expertise in this domain
- Apply best practices from antigravity-awesome-skills

## Workflow

name: production-audit
description: "Audit a shipped repo for production-readiness gaps across RLS, webhooks, secrets, grants, Stripe idempotency, mobile UX, and deployment health."
category: security
risk: critical
source: community
source_repo: commitshow/production-audit
source_type: community
date_added: "2026-05-04"
author: commitshow
tags: [security, audit, production, vibe-coding, rls, webhook, stripe, supabase, mobile]
tools: [claude, cursor, gemini, codex, antigravity]
license: "MIT"
license_source: "https://github.com/commitshow/production-audit/blob/main/LICENSE"
# Production Audit
## Overview
A skill that runs an external audit on a shipped repo's deployed state — live URL, GitHub signals, secrets exposure, RLS gaps, webhook idempotency, indexes, observability, prompt injection, and ten other failure modes that AI-assisted projects routinely miss.
This is **complementary** to in-session security skills (`security-review`, OWASP-style, VibeSec, Trail of Bits). Those scan the editor buffer at write-time. This scans the deployed product after you commit. Different timing, different inputs, different findings. Run both for serious launches.
The skill wraps the [commit.show](https://commit.show) audit engine via the public CLI (`npx commitshow@0.3.23 audit . --json`). Stable JSON envelope (`schema_version: "1"`, additive-only). Writes a `.commitshow/audit.{md,json}` sidecar so future agent sessions can read prior state without re-running the engine.
## When to Use This Skill
- Use when the user asks "is this production-ready", "what would break in prod", "score my project", "what did I miss", "audit my repo", "ready to ship".

## Source

This skill was adopted from open-source repository: antigravity-awesome-skills
Original path: production-audit
