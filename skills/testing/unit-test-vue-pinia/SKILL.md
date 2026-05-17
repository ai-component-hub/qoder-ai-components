---
name: 'unit-test-vue-pinia'
description: 'Write and review unit tests for Vue 3 + TypeScript + Vitest + Pinia codebases. Use when creating or updating tests for components, composables, and stores; mocking Pinia with createTestingPinia; appl'
version: 1.0.0
source: awesome-copilot
tier: 3
adopted: 2026-05-16
batch: bulk-adoption
---

# unit-test-vue-pinia

'Write and review unit tests for Vue 3 + TypeScript + Vitest + Pinia codebases. Use when creating or updating tests for components, composables, and stores; mocking Pinia with createTestingPinia; appl

## When to Use

- Use this skill when working on tasks related to unit test vue pinia
- Apply best practices from awesome-copilot

## Workflow

1. Identify the behavior boundary first: component UI behavior, composable behavior, or store behavior.
2. Choose the narrowest test style that can prove that behavior.
3. Set up Pinia with the least powerful option that still covers the scenario.
4. Drive the test through public inputs such as props, form updates, button clicks, emitted child events, and store APIs.
5. Assert observable outputs and side effects before considering any instance-level assertion.
6. Return or review tests with clear behavior-oriented names and note any remaining coverage gaps.

## Source

Adopted from: awesome-copilot
