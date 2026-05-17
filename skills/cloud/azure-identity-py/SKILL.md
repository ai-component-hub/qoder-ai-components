---
name: 'azure-identity-py'
description: 'Azure Identity SDK for Python authentication. Use for DefaultAzureCredential,'
adopted: 2026-05-16
batch: bulk-adoption
managed identity, service principals, and token caching.
source: antigravity-awesome-skills
tier: 4
---

# azure-identity-py

Azure Identity SDK for Python authentication. Use for DefaultAzureCredential, managed identity, service principals, and token caching.

## When to Use

- Use this skill when working on tasks related to azure identity py
- Apply best practices from antigravity-awesome-skills

## Workflow

name: azure-identity-py
description: Azure Identity SDK for Python authentication. Use for DefaultAzureCredential, managed identity, service principals, and token caching.
risk: unknown
source: community
date_added: '2026-02-27'
# Azure Identity SDK for Python
Authentication library for Azure SDK clients using Microsoft Entra ID (formerly Azure AD).
## Installation
```bash
pip install azure-identity
```
## Environment Variables
```bash
# Service Principal (for production/CI)
AZURE_TENANT_ID=<your-tenant-id>

## Source

Adopted from: antigravity-awesome-skills
