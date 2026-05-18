---
name: 'arize-ai-provider-integration'
description: 'Creates, reads, updates, and deletes Arize AI integrations that store'
adopted: 2026-05-16
LLM provider credentials used by evaluators and other Arize features. Supports any
LLM provider (e.g. OpenAI, Anthropic, Azure Ope
source: awesome-copilot
tier: 2
---

# arize-ai-provider-integration

Creates, reads, updates, and deletes Arize AI integrations that store LLM provider credentials used by evaluators and other Arize features. Supports any LLM provider (e.g. OpenAI, Anthropic, Azure Ope

## When to Use

- Use this skill when working on tasks related to arize ai provider integration
- Trigger when you need expertise in this domain
- Apply best practices from awesome-copilot

## Workflow

name: arize-ai-provider-integration
description: Creates, reads, updates, and deletes Arize AI integrations that store LLM provider credentials used by evaluators and other Arize features. Supports any LLM provider (e.g. OpenAI, Anthropic, Azure OpenAI, AWS Bedrock, Vertex AI, Gemini, NVIDIA NIM). Use when the user mentions AI integration, LLM provider credentials, create integration, list integrations, update credentials, delete integration, or connecting an LLM provider to Arize.
metadata:
  author: arize
  version: "1.0"
compatibility: Requires the ax CLI and a configured Arize profile.
# Arize AI Integration Skill
> **`SPACE`** — Most `--space` flags and the `ARIZE_SPACE` env var accept a space **name** (e.g., `my-workspace`) or a base64 space **ID** (e.g., `U3BhY2U6...`). Find yours with `ax spaces list`.
> **Note:** `ai-integrations create` does **not** accept `--space` — AI integrations are account-scoped. Use `--space` only with `list`, `get`, `update`, and `delete`.
## Concepts
- **AI Integration** = stored LLM provider credentials registered in Arize; used by evaluators to call a judge model and by other Arize features that need to invoke an LLM on your behalf
- **Provider** = the LLM service backing the integration (e.g., `openAI`, `anthropic`, `awsBedrock`)
- **Integration ID** = a base64-encoded global identifier for an integration (e.g., `TGxtSW50ZWdyYXRpb246MTI6YUJjRA==`); required for evaluator creation and other downstream operations
- **Scoping** = visibility rules controlling which spaces or users can use an integration
- **Auth type** = how Arize authenticates with the provider: `default` (provider API key), `proxy_with_headers` (proxy via custom headers), or `bearer_token` (bearer token auth)
## Prerequisites
Proceed directly with the task — run the `ax` command you need. Do NOT check versions, env vars, or profiles upfront.
If an `ax` command fails, troubleshoot based on the error:
- `command not found` or version error → see references/ax-setup.md
- `401 Unauthorized` / missing API key → run `ax profiles show` to inspect the current profile. If the profile is missing or the API key is wrong, follow references/ax-profiles.md to create/update it. If the user doesn't have their key, direct them to https://app.arize.com/admin > API Keys

## Source

This skill was adopted from open-source repository: awesome-copilot
Original path: arize-ai-provider-integration
