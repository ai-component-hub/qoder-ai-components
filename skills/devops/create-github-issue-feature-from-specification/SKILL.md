---
name: 'create-github-issue-feature-from-specification'
description: 'Create GitHub Issue for feature request from specification file using'
adopted: 2026-05-16
batch: bulk-adoption
feature_request.yml template.
source: awesome-copilot
tier: 3
---

# create-github-issue-feature-from-specification

'Create GitHub Issue for feature request from specification file using feature_request.yml template.'

## When to Use

- Use this skill when working on tasks related to create github issue feature from specification
- Apply best practices from awesome-copilot

## Workflow

name: create-github-issue-feature-from-specification
description: 'Create GitHub Issue for feature request from specification file using feature_request.yml template.'
# Create GitHub Issue from Specification
Create GitHub Issue for the specification at `${file}`.
## Process
1. Analyze specification file to extract requirements
2. Check existing issues using `search_issues`
3. Create new issue using `create_issue` or update existing with `update_issue`
4. Use `feature_request.yml` template (fallback to default)
## Requirements
- Single issue for the complete specification
- Clear title identif

## Source

Adopted from: awesome-copilot
