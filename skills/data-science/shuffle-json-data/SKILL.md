---
name: 'shuffle-json-data'
description: 'Shuffle repetitive JSON objects safely by validating schema consistency'
adopted: 2026-05-16
batch: bulk-adoption
before randomising entries.
source: awesome-copilot
tier: 3
---

# shuffle-json-data

'Shuffle repetitive JSON objects safely by validating schema consistency before randomising entries.'

## When to Use

- Use this skill when working on tasks related to shuffle json data
- Apply best practices from awesome-copilot

## Workflow

1. **Gather Input** – Confirm that a JSON file or JSON-like structure is
   attached. If not, pause and request the data file.
2. **Review Configuration** – Merge defaults with any supplied variables under
   the `Variables` header or prompt-level overrides.
3. **Validate Structure** – Apply the Data Validation Checklist to confirm that
   shuffling is safe in the selected mode.
4. **Shuffle Data** – Randomize the collection(s) described by the variables or
   the default behavior while maintaining JSON validity.
5. **Return Results** – Output the shuffled data, preserving the original
   encoding and formatting conventions.

## Source

Adopted from: awesome-copilot
