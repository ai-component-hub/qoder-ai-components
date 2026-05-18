---
name: 'azure-identity-rust'
description: 'Azure Identity SDK for Rust authentication. Use for DeveloperToolsCredential,'
adopted: 2026-05-16
batch: bulk-adoption
ManagedIdentityCredential, ClientSecretCredential, and token-based authentication.
source: antigravity-awesome-skills
tier: 3
---

# azure-identity-rust

Azure Identity SDK for Rust authentication. Use for DeveloperToolsCredential, ManagedIdentityCredential, ClientSecretCredential, and token-based authentication.

## When to Use

- Use this skill when working on tasks related to azure identity rust
- Apply best practices from antigravity-awesome-skills

## Workflow

name: azure-identity-rust
description: Azure Identity SDK for Rust authentication. Use for DeveloperToolsCredential, ManagedIdentityCredential, ClientSecretCredential, and token-based authentication.
risk: unknown
source: community
date_added: '2026-02-27'
# Azure Identity SDK for Rust
Authentication library for Azure SDK clients using Microsoft Entra ID (formerly Azure AD).
## Installation
```sh
cargo add azure_identity
```
## Environment Variables
```bash
# Service Principal (for production/CI)
AZURE_TENANT_ID=<your-tenant-id>

## Source

Adopted from: antigravity-awesome-skills
