---
name: 'arize-experiment'
description: 'Creates, runs, and analyzes Arize experiments for evaluating and comparing'
adopted: 2026-05-16
model performance. Covers experiment CRUD, exporting runs, comparing results, and
evaluation workflows using the ax CLI. Use
source: awesome-copilot
tier: 2
---

# arize-experiment

Creates, runs, and analyzes Arize experiments for evaluating and comparing model performance. Covers experiment CRUD, exporting runs, comparing results, and evaluation workflows using the ax CLI. Use 

## When to Use

- Use this skill when working on tasks related to arize experiment
- Trigger when you need expertise in this domain
- Apply best practices from awesome-copilot

## Workflow

name: arize-experiment
description: Creates, runs, and analyzes Arize experiments for evaluating and comparing model performance. Covers experiment CRUD, exporting runs, comparing results, and evaluation workflows using the ax CLI. Use when the user mentions create experiment, run experiment, compare models, model performance, evaluate AI, experiment results, benchmark, A/B test models, or measure accuracy.
metadata:
  author: arize
  version: "1.0"
compatibility: Requires the ax CLI and a configured Arize profile.
# Arize Experiment Skill
> **`SPACE`** — All `--space` flags and the `ARIZE_SPACE` env var accept a space **name** (e.g., `my-workspace`) or a base64 space **ID** (e.g., `U3BhY2U6...`). Find yours with `ax spaces list`.
## Concepts
- **Experiment** = a named evaluation run against a specific dataset version, containing one run per example
- **Experiment Run** = the result of processing one dataset example -- includes the model output, optional evaluations, and optional metadata
- **Dataset** = a versioned collection of examples; every experiment is tied to a dataset and a specific dataset version
- **Evaluation** = a named metric attached to a run (e.g., `correctness`, `relevance`), with optional label, score, and explanation
The typical flow: export a dataset → process each example → collect outputs and evaluations → create an experiment with the runs.
## Prerequisites
Proceed directly with the task — run the `ax` command you need. Do NOT check versions, env vars, or profiles upfront.
If an `ax` command fails, troubleshoot based on the error:
- `command not found` or version error → see references/ax-setup.md
- `401 Unauthorized` / missing API key → run `ax profiles show` to inspect the current profile. If the profile is missing or the API key is wrong, follow references/ax-profiles.md to create/update it. If the user doesn't have their key, direct them to https://app.arize.com/admin > API Keys
- Space unknown → run `ax spaces list` to pick by name, or ask the user

## Source

This skill was adopted from open-source repository: awesome-copilot
Original path: arize-experiment
