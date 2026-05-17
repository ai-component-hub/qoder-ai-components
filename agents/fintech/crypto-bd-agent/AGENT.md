---
name: 'crypto-bd-agent'
description: 'Production-tested patterns for building AI agents that autonomously discover,'
> evaluate, and acquire token listings for cryptocurrency exchanges.
source: open-source (antigravity-awesome-skills)
type: autonomous_agent_skill
version: 1.0
---

# Crypto Bd Agent

"Production-tested patterns for building AI agents that autonomously discover, > evaluate, and acquire token listings for cryptocurrency exchanges."

## Autonomous Capabilities

- Autonomous operation without manual intervention
- Intelligent task planning and execution
- Self-monitoring and error recovery
- Multi-step workflow orchestration

## Use Cases

- Automated task execution
- Complex workflow management
- Intelligent decision making
- Autonomous problem solving

## Workflow

1. Initialize agent with task parameters
2. Analyze task requirements
3. Execute autonomous workflow
4. Monitor progress and handle errors
5. Report results and completion status

## Source

This autonomous agent was adopted from: `antigravity-awesome-skills/skills/crypto-bd-agent/SKILL.md`

## Original Content

---
name: crypto-bd-agent
description: "Production-tested patterns for building AI agents that autonomously discover, > evaluate, and acquire token listings for cryptocurrency exchanges."
risk: safe
source: community
tags: null
date_added: '2026-02-27'
---

# Crypto BD Agent — Autonomous Business Development for Exchanges

> Production-tested patterns for building AI agents that autonomously discover,
> evaluate, and acquire token listings for cryptocurrency exchanges.

## Overview

This skill teaches AI agents systematic crypto business development: discover
promising tokens across chains, score them with a 100-point weighted system,
verify safety through wallet forensics, and manage outreach pipelines with
human-in-the-loop oversight.

Built from production experience running Buzz BD Agent by SolCex Exchange —
an autonomous agent on decentralized infrastructure with 13 intelligence
sources, x402 micropayments, and dual-chain ERC-8004 registration.

Reference implementation: https://github.com/buzzbysolcex/buzz-bd-agent

## When to Use This Skill

- Building an AI agent for crypto/DeFi business development
- Creating token evaluation and scoring systems
- Implementing multi-chain scanning pipelines
- Setting up autonomous payment workflows (x402)
- Designing wallet forensics for deployer analysis
- Managing BD pipelines with human-in-the-loop
- Registering agents on-chain via ERC-8004
- Implementing cost-efficient LLM cascades

## Do Not Use When

- Building trading bots (this is BD, not trading)
- Creating DeFi protocols or smart contracts
- Non-crypto business development

---

## Architecture
```text
Intelligence Sources (Free + Paid via x402)
        |
        v
  Scoring Engine (100-point weighted)
        |
        v
  Wallet Forensics (deployer verification)
        |
        v
  Pipeline Manager (10-stage tracked)
        |
        v
  Outreach Drafts → Human Approval → Send
```

### LLM Cascade Pattern

Route tasks to the cheapest model that handles them c
