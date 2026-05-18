---
name: 'nodejs-keccak256'
description: 'Prevent Ethereum hashing bugs in JavaScript and TypeScript. Node'
adopted: 2026-05-16
batch: bulk-adoption
is NIST SHA3, not Ethereum Keccak-256, and silently breaks selectors, signatures,
storage slots, and address derivation.
source: everything-claude-code
---

# nodejs-keccak256

Prevent Ethereum hashing bugs in JavaScript and TypeScript. Node's sha3-256 is NIST SHA3, not Ethereum Keccak-256, and silently breaks selectors, signatures, storage slots, and address derivation.

## When to Use

- Use this skill when working on tasks related to nodejs keccak256
- Apply best practices from everything-claude-code

## Workflow

name: nodejs-keccak256
description: Prevent Ethereum hashing bugs in JavaScript and TypeScript. Node's sha3-256 is NIST SHA3, not Ethereum Keccak-256, and silently breaks selectors, signatures, storage slots, and address derivation.
origin: ECC direct-port adaptation
version: "1.0.0"
# Node.js Keccak-256
Ethereum uses Keccak-256, not the NIST-standardized SHA3 variant exposed by Node's `crypto.createHash('sha3-256')`.
## When to Use
- Computing Ethereum function selectors or event topics
- Building EIP-712, signature, Merkle, or storage-slot helpers in JS/TS
- Reviewing any code that hashes Et

## Source

Adopted from: everything-claude-code
