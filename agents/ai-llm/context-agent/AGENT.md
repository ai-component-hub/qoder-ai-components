---
name: 'context-agent'
description: 'Agente de contexto para continuidade entre sessoes. Salva resumos, decisoes,'
tarefas pendentes e carrega briefing automatico na sessao seguinte.
source: open-source (antigravity-awesome-skills)
type: autonomous_agent_skill
version: 1.0
---

# Context Agent

Agente de contexto para continuidade entre sessoes. Salva resumos, decisoes, tarefas pendentes e carrega briefing automatico na sessao seguinte.

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

This autonomous agent was adopted from: `antigravity-awesome-skills/skills/context-agent/SKILL.md`

## Original Content

---
name: context-agent
description: Agente de contexto para continuidade entre sessoes. Salva resumos, decisoes, tarefas pendentes e carrega briefing automatico na sessao seguinte.
risk: safe
source: community
date_added: '2026-03-06'
author: renat
tags:
- context
- session-management
- continuity
- memory
tools:
- claude-code
- antigravity
- cursor
- gemini-cli
- codex-cli
---

# Context Agent

## Overview

Agente de contexto para continuidade entre sessoes. Salva resumos, decisoes, tarefas pendentes e carrega briefing automatico na sessao seguinte.

## When to Use This Skill

- When the user mentions "salvar contexto" or related topics
- When the user mentions "salva o contexto" or related topics
- When the user mentions "proxima sessao" or related topics
- When the user mentions "briefing sessao" or related topics
- When the user mentions "resumo sessao" or related topics
- When the user mentions "continuidade sessao" or related topics

## Do Not Use This Skill When

- The task is unrelated to context agent
- A simpler, more specific tool can handle the request
- The user needs general-purpose assistance without domain expertise

## How It Works

Continuidade perfeita entre sessões do Claude Code. Captura, comprime e
restaura contexto automaticamente — tópicos, decisões, tarefas, erros,
arquivos modificados e descobertas técnicas.

## Localização

```
C:\Users\renat\skills\context-agent\
├── SKILL.md
├── scripts/
│   ├── config.py               # Paths e constantes
│   ├── models.py               # Dataclasses
│   ├── session_parser.py       # Parser JSONL do Claude Code
│   ├── session_summary.py      # Gerador de resumos
│   ├── active_context.py       # Gerencia ACTIVE_CONTEXT.md
│   ├── project_registry.py     # Registro de projetos
│   ├── compressor.py           # Compressão e arquivamento
│   ├── search.py               # Busca FTS5
│   ├── context_loader.py       # Carrega contexto
│   └── context_manager.py      # CLI entry point
├── references/
│   ├──
