---
name: 'article-writing'
description: 'Write articles, guides, blog posts, tutorials, newsletter issues, and'
adopted: 2026-05-16
other long-form content in a distinctive voice derived from supplied examples or
brand guidance. Use when the user wants polished
source: everything-claude-code
tier: 2
---

# article-writing

Write articles, guides, blog posts, tutorials, newsletter issues, and other long-form content in a distinctive voice derived from supplied examples or brand guidance. Use when the user wants polished 

## When to Use

- Use this skill when working on tasks related to article writing
- Trigger when you need expertise in this domain
- Apply best practices from everything-claude-code

## Workflow

name: article-writing
description: Write articles, guides, blog posts, tutorials, newsletter issues, and other long-form content in a distinctive voice derived from supplied examples or brand guidance. Use when the user wants polished written content longer than a paragraph, especially when voice consistency, structure, and credibility matter.
origin: ECC
# Article Writing
Write long-form content that sounds like an actual person with a point of view, not an LLM smoothing itself into paste.
## When to Activate
- drafting blog posts, essays, launch posts, guides, tutorials, or newsletter issues
- turning notes, transcripts, or research into polished articles
- matching an existing founder, operator, or brand voice from examples
- tightening structure, pacing, and evidence in already-written long-form copy
## Core Rules
1. Lead with the concrete thing: artifact, example, output, anecdote, number, screenshot, or code.
2. Explain after the example, not before.
3. Keep sentences tight unless the source voice is intentionally expansive.
4. Use proof instead of adjectives.
5. Never invent facts, credibility, or customer evidence.
## Voice Handling
If the user wants a specific voice, run `brand-voice` first and reuse its `VOICE PROFILE`.
Do not duplicate a second style-analysis pass here unless the user explicitly asks for one.
If no voice references are given, default to a sharp operator voice: concrete, unsentimental, useful.

## Source

This skill was adopted from open-source repository: everything-claude-code
Original path: article-writing
