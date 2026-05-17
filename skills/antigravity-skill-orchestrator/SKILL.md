---
name: 'antigravity-skill-orchestrator'
description: 'A meta-skill that understands task requirements, dynamically selects'
adopted: 2026-05-16
appropriate skills, tracks successful skill combinations using agent-memory-mcp,
and prevents skill overuse for simple tasks.
source: antigravity-awesome-skills
tier: 2
---

# antigravity-skill-orchestrator

"A meta-skill that understands task requirements, dynamically selects appropriate skills, tracks successful skill combinations using agent-memory-mcp, and prevents skill overuse for simple tasks."

## When to Use

- Use this skill when working on tasks related to antigravity skill orchestrator
- Trigger when you need expertise in this domain
- Apply best practices from antigravity-awesome-skills

## Workflow

name: antigravity-skill-orchestrator
description: "A meta-skill that understands task requirements, dynamically selects appropriate skills, tracks successful skill combinations using agent-memory-mcp, and prevents skill overuse for simple tasks."
category: meta
risk: safe
source: community
tags: "[orchestration, meta-skill, agent-memory, task-evaluation]"
date_added: "2026-03-13"
# antigravity-skill-orchestrator
## Overview
The `skill-orchestrator` is a meta-skill designed to enhance the AI agent's ability to tackle complex problems. It acts as an intelligent coordinator that first evaluates the complexity of a user's request. Based on that evaluation, it determines if specialized skills are needed. If they are, it selects the right combination of skills, explicitly tracks these combinations using `@agent-memory-mcp` for future reference, and guides the agent through the execution process. Crucially, it includes strict guardrails to prevent the unnecessary use of specialized skills for simple tasks that can be solved with baseline capabilities.
## When to Use This Skill
- Use when tackling a complex, multi-step problem that likely requires multiple domains of expertise.
- Use when you are unsure which specific skills are best suited for a given user request, and need to discover them from the broader ecosystem.
- Use when the user explicitly asks to "orchestrate", "combine skills", or "use the best tools for the job" on a significant task.
- Use when you want to look up previously successful combinations of skills for a specific type of problem.
## Core Concepts
### Task Evaluation Guardrails
Not every task requires a specialized skill. For straightforward issues (e.g., small CSS fixes, simple script writing, renaming a variable), **DO NOT USE** specialized skills. Over-engineering simple tasks wastes tokens and time. 
Additionally, the orchestrator is strictly forbidden from creating new skills. Its sole purpose is to combine and use existing skills provided by the community or present in the current environment.
Before invoking any skills, evaluate the task:

## Source

This skill was adopted from open-source repository: antigravity-awesome-skills
Original path: antigravity-skill-orchestrator
