---
name: 'appinsights-instrumentation'
description: 'Instrument a webapp to send useful telemetry data to Azure App Insights'
adopted: 2026-05-16
source: awesome-copilot
tier: 2
version: 1.0.0
---

# appinsights-instrumentation

'Instrument a webapp to send useful telemetry data to Azure App Insights'

## When to Use

- Use this skill when working on tasks related to appinsights instrumentation
- Trigger when you need expertise in this domain
- Apply best practices from awesome-copilot

## Workflow

name: appinsights-instrumentation
description: 'Instrument a webapp to send useful telemetry data to Azure App Insights'
# AppInsights instrumentation
This skill enables sending telemetry data of a webapp to Azure App Insights for better observability of the app's health.
## When to use this skill
Use this skill when the user wants to enable telemetry for their webapp.
## Prerequisites
The app in the workspace must be one of these kinds
- An ASP.NET Core app hosted in Azure
- A Node.js app hosted in Azure
## Guidelines
### Collect context information
Find out the (programming language, application framework, hosting) tuple of the application the user is trying to add telemetry support in. This determines how the application can be instrumented. Read the source code to make an educated guess. Confirm with the user on anything you don't know. You must always ask the user where the application is hosted (e.g. on a personal computer, in an Azure App Service as code, in an Azure App Service as container, in an Azure Container App, etc.). 
### Prefer auto-instrument if possible
If the app is a C# ASP.NET Core app hosted in Azure App Service, use [AUTO guide](references/AUTO.md) to help user auto-instrument the app.
### Manually instrument
Manually instrument the app by creating the AppInsights resource and update the app's code. 
#### Create AppInsights resource
Use one of the following options that fits the environment.
- Add AppInsights to existing Bicep template. See [examples/appinsights.bicep](examples/appinsights.bicep) for what to add. This is the best option if there are existing Bicep template files in the workspace.

## Source

This skill was adopted from open-source repository: awesome-copilot
Original path: appinsights-instrumentation
