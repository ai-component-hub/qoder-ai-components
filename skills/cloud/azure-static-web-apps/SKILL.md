---
name: 'azure-static-web-apps'
description: 'Helps create, configure, and deploy Azure Static Web Apps using the SWA'
adopted: 2026-05-16
CLI. Use when deploying static sites to Azure, setting up SWA local development,
configuring staticwebapp.config.json, adding Az
source: awesome-copilot
tier: 2
---

# azure-static-web-apps

Helps create, configure, and deploy Azure Static Web Apps using the SWA CLI. Use when deploying static sites to Azure, setting up SWA local development, configuring staticwebapp.config.json, adding Az

## When to Use

- Use this skill when working on tasks related to azure static web apps
- Trigger when you need expertise in this domain
- Apply best practices from awesome-copilot

## Workflow

name: azure-static-web-apps
description: Helps create, configure, and deploy Azure Static Web Apps using the SWA CLI. Use when deploying static sites to Azure, setting up SWA local development, configuring staticwebapp.config.json, adding Azure Functions APIs to SWA, or setting up GitHub Actions CI/CD for Static Web Apps.
## Overview
Azure Static Web Apps (SWA) hosts static frontends with optional serverless API backends. The SWA CLI (`swa`) provides local development emulation and deployment capabilities.
**Key features:**
- Local emulator with API proxy and auth simulation
- Framework auto-detection and configuration
- Direct deployment to Azure
- Database connections support
**Config files:**
- `swa-cli.config.json` - CLI settings, **created by `swa init`** (never create manually)
- `staticwebapp.config.json` - Runtime config (routes, auth, headers, API runtime) - can be created manually
## General Instructions
### Installation
```bash
npm install -D @azure/static-web-apps-cli
```
Verify: `npx swa --version`
### Quick Start Workflow
**IMPORTANT: Always use `swa init` to create configuration files. Never manually create `swa-cli.config.json`.**

## Source

This skill was adopted from open-source repository: awesome-copilot
Original path: azure-static-web-apps
