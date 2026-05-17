---
name: 'typespec-create-agent'
description: 'Generate a complete TypeSpec declarative agent with instructions, capabilities,'
adopted: 2026-05-16
and conversation starters for Microsoft 365 Copilot
source: awesome-copilot
tier: 2
version: 1.0.0
---

# typespec-create-agent

'Generate a complete TypeSpec declarative agent with instructions, capabilities, and conversation starters for Microsoft 365 Copilot'

## When to Use

- Use this skill when working on tasks related to typespec create agent
- Trigger when you need expertise in this domain
- Apply best practices from awesome-copilot

## Workflow

name: typespec-create-agent
description: 'Generate a complete TypeSpec declarative agent with instructions, capabilities, and conversation starters for Microsoft 365 Copilot'
# Create TypeSpec Declarative Agent
Create a complete TypeSpec declarative agent for Microsoft 365 Copilot with the following structure:
## Requirements
Generate a `main.tsp` file with:
1. **Agent Declaration**
   - Use `@agent` decorator with a descriptive name and description
   - Name should be 100 characters or less
   - Description should be 1,000 characters or less
2. **Instructions**
   - Use `@instructions` decorator with clear behavioral guidelines
   - Define the agent's role, expertise, and personality
   - Specify what the agent should and shouldn't do
   - Keep under 8,000 characters
3. **Conversation Starters**
   - Include 2-4 `@conversationStarter` decorators
   - Each with a title and example query
   - Make them diverse and showcase different capabilities
4. **Capabilities** (based on user needs)

## Source

This skill was adopted from open-source repository: awesome-copilot
Original path: typespec-create-agent
