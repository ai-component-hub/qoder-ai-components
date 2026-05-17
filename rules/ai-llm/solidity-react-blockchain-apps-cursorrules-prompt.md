# Solidity React Blockchain Apps Cursorrules Prompt

**Source:** Open-source (awesome-cursorrules/rules/solidity-react-blockchain-apps-cursorrules-prompt-.mdc)  
**Adopted:** 2026-05-16

---

## Category

AI Coding Standards and Best Practices

## Rules

---
description: "Cursor rules for Solidity development with React Blockchain apps integration."
globs: **/*
alwaysApply: false
---
Solidity React Blockchain Apps Guidelines

- Prioritize secure Solidity smart contracts with explicit visibility, access control, and clear NatSpec documentation.
- Use established security tooling such as Slither, Mythril, and property-based tests for critical contract behavior.
- Prefer OpenZeppelin contracts for common primitives such as ownership, access control, multisig, and timelocks.
- Optimize gas deliberately by reviewing storage layout, function visibility, and unnecessary writes.
- Use pull-payment patterns, event logging, and defensive error handling for production-grade contracts.
- Keep Web3 frontend code type-safe and explicit when interacting with wallets, providers, and transactions.


## Validation

These rules are automatically enforced by Qoder during code generation and review.

## Notes

This rule was adopted from open-source repository and converted to Qoder format.
