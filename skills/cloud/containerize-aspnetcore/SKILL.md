---
name: 'containerize-aspnetcore'
description: 'Containerize an ASP.NET Core project by creating Dockerfile and .dockerfile'
adopted: 2026-05-16
files customized for the project.
source: awesome-copilot
tier: 2
version: 1.0.0
---

# containerize-aspnetcore

'Containerize an ASP.NET Core project by creating Dockerfile and .dockerfile files customized for the project.'

## When to Use

- Use this skill when working on tasks related to containerize aspnetcore
- Trigger when you need expertise in this domain
- Apply best practices from awesome-copilot

## Workflow

name: containerize-aspnetcore
description: 'Containerize an ASP.NET Core project by creating Dockerfile and .dockerfile files customized for the project.'
# ASP.NET Core Docker Containerization Prompt
## Containerization Request
Containerize the ASP.NET Core (.NET) project specified in the settings below, focusing **exclusively** on changes required for the application to run in a Linux Docker container. Containerization should consider all settings specified here.
Abide by best practices for containerizing .NET Core applications, ensuring that the container is optimized for performance, security, and maintainability.
## Containerization Settings
This section of the prompt contains the specific settings and configurations required for containerizing the ASP.NET Core application. Prior to running this prompt, ensure that the settings are filled out with the necessary information. Note that in many cases, only the first few settings are required. Later settings can be left as defaults if they do not apply to the project being containerized.
Any settings that are not specified will be set to default values. The default values are provided in `[square brackets]`.
### Basic Project Information
1. Project to containerize: 
   - `[ProjectName (provide path to .csproj file)]`
2. .NET version to use:
   - `[8.0 or 9.0 (Default 8.0)]`
3. Linux distribution to use:
   - `[debian, alpine, ubuntu, chiseled, or Azure Linux (mariner) (Default debian)]`
4. Custom base image for the build stage of the Docker image ("None" to use standard Microsoft base image):
   - `[Specify base image to use for build stage (Default None)]`
5. Custom base image for the run stage of the Docker image ("None" to use standard Microsoft base image):
   - `[Specify base image to use for run stage (Default None)]`   

## Source

This skill was adopted from open-source repository: awesome-copilot
Original path: containerize-aspnetcore
