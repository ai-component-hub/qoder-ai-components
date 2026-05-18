---
name: 'multi-stage-dockerfile'
description: 'Create optimized multi-stage Dockerfiles for any language or framework'
adopted: 2026-05-16
batch: bulk-adoption
source: awesome-copilot
tier: 3
version: 1.0.0
---

# multi-stage-dockerfile

'Create optimized multi-stage Dockerfiles for any language or framework'

## When to Use

- Use this skill when working on tasks related to multi stage dockerfile
- Apply best practices from awesome-copilot

## Workflow

name: multi-stage-dockerfile
description: 'Create optimized multi-stage Dockerfiles for any language or framework'
Your goal is to help me create efficient multi-stage Dockerfiles that follow best practices, resulting in smaller, more secure container images.
## Multi-Stage Structure
- Use a builder stage for compilation, dependency installation, and other build-time operations
- Use a separate runtime stage that only includes what's needed to run the application
- Copy only the necessary artifacts from the builder stage to the runtime stage
- Use meaningful stage names with the `AS` keyword (

## Source

Adopted from: awesome-copilot
