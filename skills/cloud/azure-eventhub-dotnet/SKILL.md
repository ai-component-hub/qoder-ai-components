---
name: 'azure-eventhub-dotnet'
description: 'Azure Event Hubs SDK for .NET.'
adopted: 2026-05-16
batch: bulk-adoption
source: antigravity-awesome-skills
tier: 4
version: 1.0.0
---

# azure-eventhub-dotnet

Azure Event Hubs SDK for .NET.

## When to Use

- Use this skill when working on tasks related to azure eventhub dotnet
- Apply best practices from antigravity-awesome-skills

## Workflow

name: azure-eventhub-dotnet
description: Azure Event Hubs SDK for .NET.
risk: unknown
source: community
date_added: '2026-02-27'
# Azure.Messaging.EventHubs (.NET)
High-throughput event streaming SDK for sending and receiving events via Azure Event Hubs.
## Installation
```bash
# Core package (sending and simple receiving)
dotnet add package Azure.Messaging.EventHubs
# Processor package (production receiving with checkpointing)
dotnet add package Azure.Messaging.EventHubs.Processor
# Authentication
dotnet add package Azure.Identity

## Source

Adopted from: antigravity-awesome-skills
