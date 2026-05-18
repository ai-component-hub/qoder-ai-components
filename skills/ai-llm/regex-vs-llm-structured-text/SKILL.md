---
name: 'regex-vs-llm-structured-text'
description: 'Decision framework for choosing between regex and LLM when parsing structured'
adopted: 2026-05-16
batch: bulk-adoption
text — start with regex, add LLM only for low-confidence edge cases.
source: everything-claude-code
tier: 3
---

# regex-vs-llm-structured-text

Decision framework for choosing between regex and LLM when parsing structured text — start with regex, add LLM only for low-confidence edge cases.

## When to Use

- Use this skill when working on tasks related to regex vs llm structured text
- Apply best practices from everything-claude-code

## Workflow

name: regex-vs-llm-structured-text
description: Decision framework for choosing between regex and LLM when parsing structured text — start with regex, add LLM only for low-confidence edge cases.
origin: ECC
# Regex vs LLM for Structured Text Parsing
A practical decision framework for parsing structured text (quizzes, forms, invoices, documents). The key insight: regex handles 95-98% of cases cheaply and deterministically. Reserve expensive LLM calls for the remaining edge cases.
## When to Activate
- Parsing structured text with repeating patterns (questions, forms, tables)
- Deciding between 

## Source

Adopted from: everything-claude-code
