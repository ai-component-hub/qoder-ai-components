---
name: 'foundry-agent-sync'
description: 'Create and synchronize prompt-based AI agents directly within Azure AI Foundry via REST API, from a local JSON manifest. Unlike scaffolding skills that only generate local code, this skill registers'
version: 1.0.0
source: awesome-copilot
tier: 3
adopted: 2026-05-16
batch: bulk-adoption
---

# foundry-agent-sync

"Create and synchronize prompt-based AI agents directly within Azure AI Foundry via REST API, from a local JSON manifest. Unlike scaffolding skills that only generate local code, this skill registers 

## When to Use

- Use this skill when working on tasks related to foundry agent sync
- Apply best practices from awesome-copilot

## Workflow

### Step 1 — Locate or scaffold the manifest

Search the repo for `foundry-agents.json`. If it doesn't exist, ask the user what agents they need and create the manifest.

### Step 2 — Locate or scaffold the sync script

Search for `sync-foundry-agents.ps1` or `foundry-agent-sync.sh`. If missing, create the PowerShell script using the template above, adapting:
- `$AgentNamePrefix` to match the project name
- `$ModelName` to the user's deployed model
- `$ManifestPath` to the actual manifest location

### Step 3 — Collect parameters

Ask the user for:
- Foundry project endpoint
- Subscription ID
- Model deployment name (default: `gpt-5-4`)
- Agent name prefix (default: repo name in kebab-case)

### Step 4 — Run the sync

Execute the PowerShell script with the collected parameters:

```powersh

## Source

Adopted from: awesome-copilot
