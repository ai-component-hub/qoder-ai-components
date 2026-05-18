---
name: 'm365-agents-dotnet'
description: 'Microsoft 365 Agents SDK for .NET. Build multichannel agents for Teams/M365/Copilot'
Studio with ASP.NET Core hosting, AgentApplication routing, and MSAL-based auth.
source: open-source (antigravity-awesome-skills)
type: autonomous_agent_skill
version: 1.0
---

# M365 Agents Dotnet

Microsoft 365 Agents SDK for .NET. Build multichannel agents for Teams/M365/Copilot Studio with ASP.NET Core hosting, AgentApplication routing, and MSAL-based auth.

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

This autonomous agent was adopted from: `antigravity-awesome-skills/skills/m365-agents-dotnet/SKILL.md`

## Original Content

---
name: m365-agents-dotnet
description: Microsoft 365 Agents SDK for .NET. Build multichannel agents for Teams/M365/Copilot Studio with ASP.NET Core hosting, AgentApplication routing, and MSAL-based auth.
risk: unknown
source: community
date_added: '2026-02-27'
---

# Microsoft 365 Agents SDK (.NET)

## Overview
Build enterprise agents for Microsoft 365, Teams, and Copilot Studio using the Microsoft.Agents SDK with ASP.NET Core hosting, agent routing, and MSAL-based authentication.

## Before implementation
- Use the microsoft-docs MCP to verify the latest APIs for AddAgent, AgentApplication, and authentication options.
- Confirm package versions in NuGet for the Microsoft.Agents.* packages you plan to use.

## Installation

```bash
dotnet add package Microsoft.Agents.Hosting.AspNetCore
dotnet add package Microsoft.Agents.Authentication.Msal
dotnet add package Microsoft.Agents.Storage
dotnet add package Microsoft.Agents.CopilotStudio.Client
dotnet add package Microsoft.Identity.Client.Extensions.Msal
```

## Configuration (appsettings.json)

```json
{
  "TokenValidation": {
    "Enabled": true,
    "Audiences": [
      "{{ClientId}}"
    ],
    "TenantId": "{{TenantId}}"
  },
  "AgentApplication": {
    "StartTypingTimer": false,
    "RemoveRecipientMention": false,
    "NormalizeMentions": false
  },
  "Connections": {
    "ServiceConnection": {
      "Settings": {
        "AuthType": "ClientSecret",
        "ClientId": "{{ClientId}}",
        "ClientSecret": "{{ClientSecret}}",
        "AuthorityEndpoint": "https://login.microsoftonline.com/{{TenantId}}",
        "Scopes": [
          "https://api.botframework.com/.default"
        ]
      }
    }
  },
  "ConnectionsMap": [
    {
      "ServiceUrl": "*",
      "Connection": "ServiceConnection"
    }
  ],
  "CopilotStudioClientSettings": {
    "DirectConnectUrl": "",
    "EnvironmentId": "",
    "SchemaName": "",
    "TenantId": "",
    "AppClientId": "",
    "AppClientSecret": ""
  }
}
```

## Core Workflow: ASP
