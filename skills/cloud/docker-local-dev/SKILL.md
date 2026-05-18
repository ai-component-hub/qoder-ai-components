---
name: 'docker-local-dev'
description: 'Generate Docker Compose and Dockerfile configurations for local development'
adopted: 2026-05-16
through interactive Q&A. Supports PHP/Laravel, WordPress, Drupal, Joomla, Node.js,
and Python stacks with Nginx, Supervisor/
source: awesome-ai-agent-skills
tier: 1
---

# docker-local-dev

Generate Docker Compose and Dockerfile configurations for local development through interactive Q&A. Supports PHP/Laravel, WordPress, Drupal, Joomla, Node.js, and Python stacks with Nginx, Supervisor/

## When to Use

- Use this skill when working on tasks related to docker local dev
- Trigger when you need expertise in this domain
- Apply best practices from awesome-ai-agent-skills

## Workflow

name: docker-local-dev
description: Generate Docker Compose and Dockerfile configurations for local development through interactive Q&A. Supports PHP/Laravel, WordPress, Drupal, Joomla, Node.js, and Python stacks with Nginx, Supervisor/PM2, databases, Redis, and email testing. Always asks clarifying questions before generating configurations.
context: fork
# Docker Local Development Environment Generator
## Overview
This skill helps you create optimized Docker development environments for your projects. It generates `docker-compose.yml`, `Dockerfile`, and related configurations through an interactive, question-driven workflow.
**When to use this skill:**
- Setting up a new Docker development environment
- Dockerizing an existing project for local development
- Adding services (database, Redis, email testing) to your Docker setup
- Updating or merging with existing Docker configurations
**Key Principle:** This skill ALWAYS asks questions before making decisions. You will be notified about each configuration choice and can adjust settings to match your exact needs.
## Important Notice
This skill uses an **interactive approach**. Before generating any files, I will:
1. Run auto-detection scripts to identify your tech stack (saves AI tokens)
2. Present the detection results for your confirmation
3. Ask 10-15 clarifying questions about your preferences
4. Show you a preview before creating or modifying files
**Why this approach?** Docker configurations are project-specific. Asking questions ensures the setup matches YOUR requirements, not generic defaults. This prevents issues and saves debugging time later.
## Quick Start

## Source

This skill was adopted from open-source repository: awesome-ai-agent-skills
Original path: docker-local-dev
