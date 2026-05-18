---
name: 'azd-deployment'
description: 'Deploy containerized frontend + backend applications to Azure Container'
adopted: 2026-05-16
batch: bulk-adoption
Apps with remote builds, managed identity, and idempotent infrastructure.
source: antigravity-awesome-skills
tier: 4
---

# azd-deployment

"Deploy containerized frontend + backend applications to Azure Container Apps with remote builds, managed identity, and idempotent infrastructure."

## When to Use

- Use this skill when working on tasks related to azd deployment
- Apply best practices from antigravity-awesome-skills

## Workflow

name: azd-deployment
description: "Deploy containerized frontend + backend applications to Azure Container Apps with remote builds, managed identity, and idempotent infrastructure."
risk: critical
source: community
date_added: "2026-02-27"
# Azure Developer CLI (azd) Container Apps Deployment
Deploy containerized frontend + backend applications to Azure Container Apps with remote builds, managed identity, and idempotent infrastructure.
## Quick Start
```bash
# Initialize and deploy
azd auth login
azd init                    # Creates azure.yaml and .azure/ folder
azd env new <env-name>      # 

## Source

Adopted from: antigravity-awesome-skills
