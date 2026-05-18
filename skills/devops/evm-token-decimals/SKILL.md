---
name: 'evm-token-decimals'
description: 'Prevent silent decimal mismatch bugs across EVM chains. Covers runtime'
adopted: 2026-05-16
decimal lookup, chain-aware caching, bridged-token precision drift, and safe normalization
for bots, dashboards, and DeFi tools.
source: everything-claude-code
tier: 2
---

# evm-token-decimals

Prevent silent decimal mismatch bugs across EVM chains. Covers runtime decimal lookup, chain-aware caching, bridged-token precision drift, and safe normalization for bots, dashboards, and DeFi tools.

## When to Use

- Use this skill when working on tasks related to evm token decimals
- Trigger when you need expertise in this domain
- Apply best practices from everything-claude-code

## Workflow

name: evm-token-decimals
description: Prevent silent decimal mismatch bugs across EVM chains. Covers runtime decimal lookup, chain-aware caching, bridged-token precision drift, and safe normalization for bots, dashboards, and DeFi tools.
origin: ECC direct-port adaptation
version: "1.0.0"
# EVM Token Decimals
Silent decimal mismatches are one of the easiest ways to ship balances or USD values that are off by orders of magnitude without throwing an error.
## When to Use
- Reading ERC-20 balances in Python, TypeScript, or Solidity
- Calculating fiat values from on-chain balances
- Comparing token amounts across multiple EVM chains
- Handling bridged assets
- Building portfolio trackers, bots, or aggregators
## How It Works
Never assume stablecoins use the same decimals everywhere. Query `decimals()` at runtime, cache by `(chain_id, token_address)`, and use decimal-safe math for value calculations.
## Examples
### Query decimals at runtime
```python
from decimal import Decimal
from web3 import Web3
ERC20_ABI = [

## Source

This skill was adopted from open-source repository: everything-claude-code
Original path: evm-token-decimals
