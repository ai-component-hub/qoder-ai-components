---
name: 'azure-ai-agents-persistent-java'
description: 'Azure AI Agents Persistent SDK for Java. Low-level SDK for creating and'
managing AI agents with threads, messages, runs, and tools.
source: open-source (antigravity-awesome-skills)
type: autonomous_agent_skill
version: 1.0
---

# Azure Ai Agents Persistent Java

Azure AI Agents Persistent SDK for Java. Low-level SDK for creating and managing AI agents with threads, messages, runs, and tools.

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

This autonomous agent was adopted from: `antigravity-awesome-skills/skills/azure-ai-agents-persistent-java/SKILL.md`

## Original Content

---
name: azure-ai-agents-persistent-java
description: Azure AI Agents Persistent SDK for Java. Low-level SDK for creating and managing AI agents with threads, messages, runs, and tools.
risk: unknown
source: community
date_added: '2026-02-27'
---

# Azure AI Agents Persistent SDK for Java

Low-level SDK for creating and managing persistent AI agents with threads, messages, runs, and tools.

## Installation

```xml
<dependency>
    <groupId>com.azure</groupId>
    <artifactId>azure-ai-agents-persistent</artifactId>
    <version>1.0.0-beta.1</version>
</dependency>
```

## Environment Variables

```bash
PROJECT_ENDPOINT=https://<resource>.services.ai.azure.com/api/projects/<project>
MODEL_DEPLOYMENT_NAME=gpt-4o-mini
```

## Authentication

```java
import com.azure.ai.agents.persistent.PersistentAgentsClient;
import com.azure.ai.agents.persistent.PersistentAgentsClientBuilder;
import com.azure.identity.DefaultAzureCredentialBuilder;

String endpoint = System.getenv("PROJECT_ENDPOINT");
PersistentAgentsClient client = new PersistentAgentsClientBuilder()
    .endpoint(endpoint)
    .credential(new DefaultAzureCredentialBuilder().build())
    .buildClient();
```

## Key Concepts

The Azure AI Agents Persistent SDK provides a low-level API for managing persistent agents that can be reused across sessions.

### Client Hierarchy

| Client | Purpose |
|--------|---------|
| `PersistentAgentsClient` | Sync client for agent operations |
| `PersistentAgentsAsyncClient` | Async client for agent operations |

## Core Workflow

### 1. Create Agent

```java
// Create agent with tools
PersistentAgent agent = client.createAgent(
    modelDeploymentName,
    "Math Tutor",
    "You are a personal math tutor."
);
```

### 2. Create Thread

```java
PersistentAgentThread thread = client.createThread();
```

### 3. Add Message

```java
client.createMessage(
    thread.getId(),
    MessageRole.USER,
    "I need help with equations."
);
```

### 4. Run Agent

```java
ThreadRun run = client.c
