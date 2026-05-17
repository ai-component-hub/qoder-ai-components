---
name: 'm365-agents-ts'
description: 'Microsoft 365 Agents SDK for TypeScript/Node.js.'
source: open-source (antigravity-awesome-skills)
type: autonomous_agent_skill
version: 1.0
---

# M365 Agents Ts

Microsoft 365 Agents SDK for TypeScript/Node.js.

## Autonomous Capabilities

- Autonomous operation without manual intervention
- Intelligent task planning and execution
- Self-monitoring and error recovery
- Multi-step workflow orchestration

## Use Cases

- Automated task execution
- Complex workflow management
- Intelligent decision making
- Autonomous problem solving

## Workflow

1. Initialize agent with task parameters
2. Analyze task requirements
3. Execute autonomous workflow
4. Monitor progress and handle errors
5. Report results and completion status

## Source

This autonomous agent was adopted from: `antigravity-awesome-skills/skills/m365-agents-ts/SKILL.md`

## Original Content

---
name: m365-agents-ts
description: Microsoft 365 Agents SDK for TypeScript/Node.js.
risk: unknown
source: community
date_added: '2026-02-27'
---

# Microsoft 365 Agents SDK (TypeScript)

Build enterprise agents for Microsoft 365, Teams, and Copilot Studio using the Microsoft 365 Agents SDK with Express hosting, AgentApplication routing, streaming responses, and Copilot Studio client integrations.

## Before implementation
- Use the microsoft-docs MCP to verify the latest API signatures for AgentApplication, startServer, and CopilotStudioClient.
- Confirm package versions on npm before wiring up samples or templates.

## Installation

```bash
npm install @microsoft/agents-hosting @microsoft/agents-hosting-express @microsoft/agents-activity
npm install @microsoft/agents-copilotstudio-client
```

## Environment Variables

```bash
PORT=3978
AZURE_RESOURCE_NAME=<azure-openai-resource>
AZURE_API_KEY=<azure-openai-key>
AZURE_OPENAI_DEPLOYMENT_NAME=gpt-4o-mini

TENANT_ID=<tenant-id>
CLIENT_ID=<client-id>
CLIENT_SECRET=<client-secret>

COPILOT_ENVIRONMENT_ID=<environment-id>
COPILOT_SCHEMA_NAME=<schema-name>
COPILOT_CLIENT_ID=<copilot-app-client-id>
COPILOT_BEARER_TOKEN=<copilot-jwt>
```

## Core Workflow: Express-hosted AgentApplication

```typescript
import { AgentApplication, TurnContext, TurnState } from "@microsoft/agents-hosting";
import { startServer } from "@microsoft/agents-hosting-express";

const agent = new AgentApplication<TurnState>();

agent.onConversationUpdate("membersAdded", async (context: TurnContext) => {
  await context.sendActivity("Welcome to the agent.");
});

agent.onMessage("hello", async (context: TurnContext) => {
  await context.sendActivity(`Echo: ${context.activity.text}`);
});

startServer(agent);
```

## Streaming responses with Azure OpenAI

```typescript
import { azure } from "@ai-sdk/azure";
import { AgentApplication, TurnContext, TurnState } from "@microsoft/agents-hosting";
import { startServer } from "@microsoft/agents-hosting-expre
