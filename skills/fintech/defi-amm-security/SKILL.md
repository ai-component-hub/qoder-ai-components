---
name: 'defi-amm-security'
description: 'Security checklist for Solidity AMM contracts, liquidity pools, and swap'
adopted: 2026-05-16
flows. Covers reentrancy, CEI ordering, donation or inflation attacks, oracle manipulation,
slippage, admin controls, and integ
source: everything-claude-code
tier: 2
---

# defi-amm-security

Security checklist for Solidity AMM contracts, liquidity pools, and swap flows. Covers reentrancy, CEI ordering, donation or inflation attacks, oracle manipulation, slippage, admin controls, and integ

## When to Use

- Use this skill when working on tasks related to defi amm security
- Trigger when you need expertise in this domain
- Apply best practices from everything-claude-code

## Workflow

name: defi-amm-security
description: Security checklist for Solidity AMM contracts, liquidity pools, and swap flows. Covers reentrancy, CEI ordering, donation or inflation attacks, oracle manipulation, slippage, admin controls, and integer math.
origin: ECC direct-port adaptation
version: "1.0.0"
# DeFi AMM Security
Critical vulnerability patterns and hardened implementations for Solidity AMM contracts, LP vaults, and swap functions.
## When to Use
- Writing or auditing a Solidity AMM or liquidity-pool contract
- Implementing swap, deposit, withdraw, mint, or burn flows that hold token balances
- Reviewing any contract that uses `token.balanceOf(address(this))` in share or reserve math
- Adding fee setters, pausers, oracle updates, or other admin functions to a DeFi protocol
## How It Works
Use this as a checklist-plus-pattern library. Review every user entrypoint against the categories below and prefer the hardened examples over hand-rolled variants.
## Execution Safety
The shell commands in this skill are local audit examples. Run them only in a trusted checkout or disposable sandbox, and do not splice untrusted contract names, paths, RPC URLs, private keys, or user-supplied flags into shell commands. Ask before installing tools or running long fuzzing/static-analysis jobs that may consume significant local or paid resources.
Never include secrets, private keys, seed phrases, API tokens, or mainnet signing credentials in command examples, logs, or reports.
## Examples
### Reentrancy: enforce CEI order
Vulnerable:
```solidity

## Source

This skill was adopted from open-source repository: everything-claude-code
Original path: defi-amm-security
