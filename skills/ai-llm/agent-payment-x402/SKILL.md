---
name: 'agent-payment-x402'
description: 'Add x402 payment execution to AI agents with per-task budgets, spending'
adopted: 2026-05-16
controls, and non-custodial wallets. Supports Base through agentwallet-sdk and X
Layer through OKX Payments / OKX Agent Payments
source: everything-claude-code
tier: 2
---

# agent-payment-x402

Add x402 payment execution to AI agents with per-task budgets, spending controls, and non-custodial wallets. Supports Base through agentwallet-sdk and X Layer through OKX Payments / OKX Agent Payments

## When to Use

- Use this skill when working on tasks related to agent payment x402
- Trigger when you need expertise in this domain
- Apply best practices from everything-claude-code

## Workflow

name: agent-payment-x402
description: Add x402 payment execution to AI agents with per-task budgets, spending controls, and non-custodial wallets. Supports Base through agentwallet-sdk and X Layer through OKX Payments / OKX Agent Payments Protocol.
origin: community
# Agent Payment Execution (x402)
Enable AI agents to make policy-gated payments with built-in spending controls. Uses the x402 HTTP payment protocol and MCP tools so agents can pay for external services, APIs, or other agents without custodial risk.
## When to Use
Use when: your agent needs to pay for an API call, purchase a service, settle with another agent, enforce per-task spending limits, or manage a non-custodial wallet. Pairs naturally with cost-aware-llm-pipeline and security-review skills.
## Decision Tree
Choose the integration path based on whether your agent is buying access to a paid API or charging others for one:
| Need | Recommended path |
|------|------------------|
| Agent pays a 402-gated API on Base or another agentwallet-supported chain | Use `agentwallet-sdk` as an MCP payment server with strict spending policy |
| Agent pays a 402-gated API on X Layer | Use OKX Agent Payments Protocol from `okx/onchainos-skills`; `okx-x402-payment` is a deprecated legacy alias |
| TypeScript API charges agents | Use OKX Payments TypeScript seller SDK docs for Express, Hono, Fastify, or Next.js |
| Go API charges agents | Use OKX Payments Go seller SDK docs for Gin, Echo, or `net/http` |
| Rust API charges agents | Use OKX Payments Rust seller SDK docs for Axum |
| Java API charges agents | Use OKX Payments Java seller SDK docs for Spring Boot 2/3, Java EE, or Jakarta |
| Python API charges agents | Check the current OKX Payments repository before implementation; a Python seller guide may not be available |
## Supported Networks
- `agentwallet-sdk`: use the package docs to confirm current network coverage before production. Base Sepolia is the safest development default; Base mainnet is the production path called out by the original skill.

## Source

This skill was adopted from open-source repository: everything-claude-code
Original path: agent-payment-x402
