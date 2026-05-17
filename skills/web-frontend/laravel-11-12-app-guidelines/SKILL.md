---
name: 'laravel-11-12-app-guidelines'
description: 'Guidelines and workflow for working on Laravel 11 or Laravel 12 applications'
adopted: 2026-05-16
across common stacks (API-only or full-stack), including optional Docker Compose/Sail,
Inertia + React, Livewire, Vue, Blad
source: awesome-ai-agent-skills
tier: 1
---

# laravel-11-12-app-guidelines

Guidelines and workflow for working on Laravel 11 or Laravel 12 applications across common stacks (API-only or full-stack), including optional Docker Compose/Sail, Inertia + React, Livewire, Vue, Blad

## When to Use

- Use this skill when working on tasks related to laravel 11 12 app guidelines
- Trigger when you need expertise in this domain
- Apply best practices from awesome-ai-agent-skills

## Workflow

name: laravel-11-12-app-guidelines
description: Guidelines and workflow for working on Laravel 11 or Laravel 12 applications across common stacks (API-only or full-stack), including optional Docker Compose/Sail, Inertia + React, Livewire, Vue, Blade, Tailwind v4, Fortify, Wayfinder, PHPUnit, Pint, and Laravel Boost MCP tools. Use when implementing features, fixing bugs, or making UI/backend changes while following project-specific instructions (AGENTS.md, docs/).
context: fork
# Laravel 11/12 App Guidelines
## Overview
Apply a consistent workflow for Laravel 11/12 apps with optional frontend stacks, Dockerized commands, and Laravel Boost tooling.
## Quick Start
- Read repository instructions first: `AGENTS.md`. If `docs/` exists, read `docs/README.md` and relevant module docs before decisions.
- Detect the stack and command locations; do not guess.
- Use Laravel Boost `search-docs` for Laravel ecosystem guidance; use Context7 only if Boost docs are unavailable.
- Follow repo conventions for naming, UI language, docs-first policies, and existing component patterns.
## Stack Detection
- Check `composer.json`, `package.json`, `docker-compose.*`, and `config/*` to confirm:
  - Docker Compose/Sail vs host commands
  - API-only vs full-stack
  - Frontend framework (Inertia/React, Livewire, Vue, Blade)
  - Auth (Fortify, Sanctum, Passport, custom)
## Laravel 11/12 Core Conventions
- Use the Laravel 11/12 structure: configure middleware, exceptions, and routes in `bootstrap/app.php`; service providers in `bootstrap/providers.php`; console configuration in `routes/console.php`.
- Use Eloquent models and relationships first; avoid raw queries and `DB::` unless truly necessary.

## Source

This skill was adopted from open-source repository: awesome-ai-agent-skills
Original path: laravel-11-12-app-guidelines
