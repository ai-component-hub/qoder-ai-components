---
name: 'cost-aware-llm-pipeline'
description: 'Cost optimization patterns for LLM API usage — model routing by task'
adopted: 2026-05-16
complexity, budget tracking, retry logic, and prompt caching.
source: everything-claude-code
tier: 2
version: 1.0.0
---

# cost-aware-llm-pipeline

Cost optimization patterns for LLM API usage — model routing by task complexity, budget tracking, retry logic, and prompt caching.

## When to Use

- Use this skill when working on tasks related to cost aware llm pipeline
- Trigger when you need expertise in this domain
- Apply best practices from everything-claude-code

## Workflow

name: cost-aware-llm-pipeline
description: Cost optimization patterns for LLM API usage — model routing by task complexity, budget tracking, retry logic, and prompt caching.
origin: ECC
# Cost-Aware LLM Pipeline
Patterns for controlling LLM API costs while maintaining quality. Combines model routing, budget tracking, retry logic, and prompt caching into a composable pipeline.
## When to Activate
- Building applications that call LLM APIs (Claude, GPT, etc.)
- Processing batches of items with varying complexity
- Need to stay within a budget for API spend
- Optimizing cost without sacrificing quality on complex tasks
## Core Concepts
### 1. Model Routing by Task Complexity
Automatically select cheaper models for simple tasks, reserving expensive models for complex ones.
```python
MODEL_SONNET = "claude-sonnet-4-6"
MODEL_HAIKU = "claude-haiku-4-5-20251001"
_SONNET_TEXT_THRESHOLD = 10_000  # chars
_SONNET_ITEM_THRESHOLD = 30     # items
def select_model(
    text_length: int,

## Source

This skill was adopted from open-source repository: everything-claude-code
Original path: cost-aware-llm-pipeline
