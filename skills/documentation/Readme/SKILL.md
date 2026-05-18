---
name: 'Readme'
description: 'Readme'
adopted: 2026-05-16
source: awesome-ai-agent-skills
tier: 1
version: 1.0.0
---

# Readme

# design-system-generator

## When to Use

- Use this skill when working on tasks related to Readme
- Trigger when you need expertise in this domain
- Apply best practices from awesome-ai-agent-skills

## Workflow

# design-system-generator
Generates a project-specific `DESIGN_SYSTEM.md` so UI/UX stays consistent across pages, components, and teams.
## What this skill produces
- `DESIGN_SYSTEM.md` (primary output)
- Optional:
  - `tokens.css` (CSS variables)
  - `design-tokens.json` (token export)
  - Example manifest snippet / guidance (cache-busting)
## What this skill optimizes for
- Component-based design that works in:
  - SPAs (React/Vue/Svelte/Angular)
  - Traditional server-rendered sites (Laravel/Rails/Django/WordPress)
  - Hybrid setups
- Accessibility defaults (focus, keyboard, contrast, reduced motion)
- Production readiness (hashed assets + manifest, minification, image optimization)
## Where to place outputs
- `DESIGN_SYSTEM.md` → repo root
- Optional token files:
  - `styles/tokens.css`
  - `styles/design-tokens.json`

## Source

This skill was adopted from open-source repository: awesome-ai-agent-skills
Original path: Readme
