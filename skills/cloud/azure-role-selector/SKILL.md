---
name: 'azure-role-selector'
description: 'When user is asking for guidance for which role to assign to an identity'
adopted: 2026-05-16
batch: bulk-adoption
given desired permissions, this agent helps them understand the role that will meet
the requirements with least privilege acces
source: awesome-copilot
---

# azure-role-selector

When user is asking for guidance for which role to assign to an identity given desired permissions, this agent helps them understand the role that will meet the requirements with least privilege acces

## When to Use

- Use this skill when working on tasks related to azure role selector
- Apply best practices from awesome-copilot

## Workflow

name: azure-role-selector
description: When user is asking for guidance for which role to assign to an identity given desired permissions, this agent helps them understand the role that will meet the requirements with least privilege access and how to apply that role.
allowed-tools: ['Azure MCP/documentation', 'Azure MCP/bicepschema', 'Azure MCP/extension_cli_generate', 'Azure MCP/get_bestpractices']
Use 'Azure MCP/documentation' tool to find the minimal role definition that matches the desired permissions the user wants to assign to an identity (If no built-in role matches the desired permiss

## Source

Adopted from: awesome-copilot
