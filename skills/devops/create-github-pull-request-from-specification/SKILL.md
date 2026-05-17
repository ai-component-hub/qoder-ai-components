---
name: 'create-github-pull-request-from-specification'
description: 'Create GitHub Pull Request for feature request from specification file'
adopted: 2026-05-16
batch: bulk-adoption
using pull_request_template.md template.
source: awesome-copilot
tier: 3
---

# create-github-pull-request-from-specification

'Create GitHub Pull Request for feature request from specification file using pull_request_template.md template.'

## When to Use

- Use this skill when working on tasks related to create github pull request from specification
- Apply best practices from awesome-copilot

## Workflow

name: create-github-pull-request-from-specification
description: 'Create GitHub Pull Request for feature request from specification file using pull_request_template.md template.'
# Create GitHub Pull Request from Specification
Create GitHub Pull Request for the specification at `${workspaceFolder}/.github/pull_request_template.md` .
## Process
1. Analyze specification file template from '${workspaceFolder}/.github/pull_request_template.md' to extract requirements by 'search' tool.
2. Create pull request draft template by using 'create_pull_request' tool on to `${input:targetBranch}`. and make 

## Source

Adopted from: awesome-copilot
