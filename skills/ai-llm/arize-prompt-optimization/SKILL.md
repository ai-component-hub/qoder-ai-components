---
name: 'arize-prompt-optimization'
description: 'Optimizes, improves, and debugs LLM prompts using production trace data,'
adopted: 2026-05-16
evaluations, and annotations. Extracts prompts from spans, gathers performance signal,
and runs a data-driven optimization loop
source: awesome-copilot
tier: 2
---

# arize-prompt-optimization

Optimizes, improves, and debugs LLM prompts using production trace data, evaluations, and annotations. Extracts prompts from spans, gathers performance signal, and runs a data-driven optimization loop

## When to Use

- Use this skill when working on tasks related to arize prompt optimization
- Trigger when you need expertise in this domain
- Apply best practices from awesome-copilot

## Workflow

name: arize-prompt-optimization
description: Optimizes, improves, and debugs LLM prompts using production trace data, evaluations, and annotations. Extracts prompts from spans, gathers performance signal, and runs a data-driven optimization loop using the ax CLI. Use when the user mentions optimize prompt, improve prompt, make AI respond better, improve output quality, prompt engineering, prompt tuning, or system prompt improvement.
metadata:
  author: arize
  version: "1.0"
compatibility: Requires the ax CLI and a configured Arize profile.
# Arize Prompt Optimization Skill
> **`SPACE`** — All `--space` flags and the `ARIZE_SPACE` env var accept a space **name** (e.g., `my-workspace`) or a base64 space **ID** (e.g., `U3BhY2U6...`). Find yours with `ax spaces list`.
## Concepts
### Where Prompts Live in Trace Data
LLM applications emit spans following OpenInference semantic conventions. Prompts are stored in different span attributes depending on the span kind and instrumentation:
| Column | What it contains | When to use |
|--------|-----------------|-------------|
| `attributes.llm.input_messages` | Structured chat messages (system, user, assistant, tool) in role-based format | **Primary source** for chat-based LLM prompts |
| `attributes.llm.input_messages.roles` | Array of roles: `system`, `user`, `assistant`, `tool` | Extract individual message roles |
| `attributes.llm.input_messages.contents` | Array of message content strings | Extract message text |
| `attributes.input.value` | Serialized prompt or user question (generic, all span kinds) | Fallback when structured messages are not available |
| `attributes.llm.prompt_template.template` | Template with `{variable}` placeholders (e.g., `"Answer {question} using {context}"`) | When the app uses prompt templates |
| `attributes.llm.prompt_template.variables` | Template variable values (JSON object) | See what values were substituted into the template |
| `attributes.output.value` | Model response text | See what the LLM produced |

## Source

This skill was adopted from open-source repository: awesome-copilot
Original path: arize-prompt-optimization
