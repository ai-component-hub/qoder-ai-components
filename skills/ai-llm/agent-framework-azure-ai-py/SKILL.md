---
name: 'agent-framework-azure-ai-py'
description: 'Build persistent agents on Azure AI Foundry using the Microsoft Agent'
adopted: 2026-05-16
batch: bulk-adoption
Framework Python SDK.
source: antigravity-awesome-skills
tier: 4
---

# agent-framework-azure-ai-py

"Build persistent agents on Azure AI Foundry using the Microsoft Agent Framework Python SDK."

## When to Use

- Use this skill when working on tasks related to agent framework azure ai py
- Apply best practices from antigravity-awesome-skills

## Workflow

name: agent-framework-azure-ai-py
description: "Build persistent agents on Azure AI Foundry using the Microsoft Agent Framework Python SDK."
risk: unknown
source: community
date_added: "2026-02-27"
# Agent Framework Azure Hosted Agents
Build persistent agents on Azure AI Foundry using the Microsoft Agent Framework Python SDK.
## Architecture
```
User Query → AzureAIAgentsProvider → Azure AI Agent Service (Persistent)
                    ↓
              Agent.run() / Agent.run_stream()
                    ↓
              Tools: Functions | Hosted (Code/Search/Web) | MCP
                    ↓

## Source

Adopted from: antigravity-awesome-skills
