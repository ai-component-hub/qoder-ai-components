---
name: 'azure-resource-health-diagnose'
description: 'Analyze Azure resource health, diagnose issues from logs and telemetry,'
adopted: 2026-05-16
and create a remediation plan for identified problems.
source: awesome-copilot
tier: 2
version: 1.0.0
---

# azure-resource-health-diagnose

'Analyze Azure resource health, diagnose issues from logs and telemetry, and create a remediation plan for identified problems.'

## When to Use

- Use this skill when working on tasks related to azure resource health diagnose
- Trigger when you need expertise in this domain
- Apply best practices from awesome-copilot

## Workflow

name: azure-resource-health-diagnose
description: 'Analyze Azure resource health, diagnose issues from logs and telemetry, and create a remediation plan for identified problems.'
# Azure Resource Health & Issue Diagnosis
This workflow analyzes a specific Azure resource to assess its health status, diagnose potential issues using logs and telemetry data, and develop a comprehensive remediation plan for any problems discovered.
## Prerequisites
- Azure MCP server configured and authenticated
- Target Azure resource identified (name and optionally resource group/subscription)
- Resource must be deployed and running to generate logs/telemetry
- Prefer Azure MCP tools (`azmcp-*`) over direct Azure CLI when available
## Workflow Steps
### Step 1: Get Azure Best Practices
**Action**: Retrieve diagnostic and troubleshooting best practices
**Tools**: Azure MCP best practices tool
**Process**:
1. **Load Best Practices**:
   - Execute Azure best practices tool to get diagnostic guidelines
   - Focus on health monitoring, log analysis, and issue resolution patterns
   - Use these practices to inform diagnostic approach and remediation recommendations
### Step 2: Resource Discovery & Identification
**Action**: Locate and identify the target Azure resource

## Source

This skill was adopted from open-source repository: awesome-copilot
Original path: azure-resource-health-diagnose
