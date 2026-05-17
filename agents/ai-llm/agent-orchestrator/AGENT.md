---
name: 'agent-orchestrator'
description: 'Meta-skill que orquestra todos os agentes do ecossistema. Scan automatico'
de skills, match por capacidades, coordenacao de workflows multi-skill e registry
management.
source: open-source (antigravity-awesome-skills)
type: autonomous_agent_skill
version: 1.0
---

# Agent Orchestrator

Meta-skill que orquestra todos os agentes do ecossistema. Scan automatico de skills, match por capacidades, coordenacao de workflows multi-skill e registry management.

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

This autonomous agent was adopted from: `antigravity-awesome-skills/skills/agent-orchestrator/SKILL.md`

## Original Content

---
name: agent-orchestrator
description: Meta-skill que orquestra todos os agentes do ecossistema. Scan automatico de skills, match por capacidades, coordenacao de workflows multi-skill e registry management.
risk: safe
source: community
date_added: '2026-03-06'
author: renat
tags:
- orchestration
- multi-agent
- workflow
- automation
tools:
- claude-code
- antigravity
- cursor
- gemini-cli
- codex-cli
---

# Agent Orchestrator

## Overview

Meta-skill que orquestra todos os agentes do ecossistema. Scan automatico de skills, match por capacidades, coordenacao de workflows multi-skill e registry management.

## When to Use This Skill

- When you need specialized assistance with this domain

## Do Not Use This Skill When

- The task is unrelated to agent orchestrator
- A simpler, more specific tool can handle the request
- The user needs general-purpose assistance without domain expertise

## How It Works

Meta-skill que funciona como camada central de decisao e coordenacao para todo
o ecossistema de skills. Faz varredura automatica, identifica agentes relevantes
e orquestra multiplos skills para tarefas complexas.

## Principio: Zero Intervencao Manual

- **SEMPRE faz varredura** antes de processar qualquer solicitacao
- Novas skills sao **auto-detectadas e incluidas** ao criar SKILL.md em qualquer subpasta
- Skills removidas sao **auto-excluidas** do registry
- Nenhum comando manual e necessario para registrar novas skills

---

## Workflow Obrigatorio (Toda Solicitacao)

Execute estes passos ANTES de processar qualquer request do usuario.
Os scripts usam paths relativos automaticamente - funciona de qualquer diretorio.

## Passo 1: Auto-Discovery (Varredura)

```bash
python agent-orchestrator/scripts/scan_registry.py
```

Ultra-rapido (<100ms) via cache de hashes MD5. So re-processa arquivos alterados.
Retorna JSON com resumo de todos os skills encontrados.

## Passo 2: Match De Skills

```bash
python agent-orchestrator/scripts/match_skills.py "<solicitacao do usu
