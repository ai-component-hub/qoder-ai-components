---
name: 'circleci-automation'
description: 'Automate CircleCI tasks via Rube MCP (Composio): trigger pipelines,'
adopted: 2026-05-16
batch: bulk-adoption
monitor workflows/jobs, retrieve artifacts and test metadata. Always search tools
first for current schemas.'
source: antigravity-awesome-skills
---

# circleci-automation

"Automate CircleCI tasks via Rube MCP (Composio): trigger pipelines, monitor workflows/jobs, retrieve artifacts and test metadata. Always search tools first for current schemas."

## When to Use

- Use this skill when working on tasks related to circleci automation
- Apply best practices from antigravity-awesome-skills

## Workflow

name: circleci-automation
description: "Automate CircleCI tasks via Rube MCP (Composio): trigger pipelines, monitor workflows/jobs, retrieve artifacts and test metadata. Always search tools first for current schemas."
risk: critical
source: community
date_added: "2026-02-27"
# CircleCI Automation via Rube MCP
Automate CircleCI CI/CD operations through Composio's CircleCI toolkit via Rube MCP.
## Prerequisites
- Rube MCP must be connected (RUBE_SEARCH_TOOLS available)
- Active CircleCI connection via `RUBE_MANAGE_CONNECTIONS` with toolkit `circleci`
- Always call `RUBE_SEARCH_TOOLS` first to ge

## Source

Adopted from: antigravity-awesome-skills
