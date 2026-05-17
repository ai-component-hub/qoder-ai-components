---
name: 'llm-trading-agent-security'
description: 'Security patterns for autonomous trading agents with wallet or transaction'
adopted: 2026-05-16
authority. Covers prompt injection, spend limits, pre-send simulation, circuit breakers,
MEV protection, and key handling.
source: everything-claude-code
tier: 2
---

# llm-trading-agent-security

Security patterns for autonomous trading agents with wallet or transaction authority. Covers prompt injection, spend limits, pre-send simulation, circuit breakers, MEV protection, and key handling.

## When to Use

- Use this skill when working on tasks related to llm trading agent security
- Trigger when you need expertise in this domain
- Apply best practices from everything-claude-code

## Workflow

name: llm-trading-agent-security
description: Security patterns for autonomous trading agents with wallet or transaction authority. Covers prompt injection, spend limits, pre-send simulation, circuit breakers, MEV protection, and key handling.
origin: ECC direct-port adaptation
version: "1.0.0"
# LLM Trading Agent Security
Autonomous trading agents have a harsher threat model than normal LLM apps: an injection or bad tool path can turn directly into asset loss.
## When to Use
- Building an AI agent that signs and sends transactions
- Auditing a trading bot or on-chain execution assistant
- Designing wallet key management for an agent
- Giving an LLM access to order placement, swaps, or treasury operations
## How It Works
Layer the defenses. No single check is enough. Treat prompt hygiene, spend policy, simulation, execution limits, and wallet isolation as independent controls.
## Examples
### Treat prompt injection as a financial attack
```python
import re
INJECTION_PATTERNS = [
    r'ignore (previous|all) instructions',
    r'new (task|directive|instruction)',

## Source

This skill was adopted from open-source repository: everything-claude-code
Original path: llm-trading-agent-security
