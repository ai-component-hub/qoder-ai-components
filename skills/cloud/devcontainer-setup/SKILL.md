---
name: 'devcontainer-setup'
description: 'Creates devcontainers with Claude Code, language-specific tooling (Python/Node/Rust/Go),'
adopted: 2026-05-16
batch: bulk-adoption
and persistent volumes. Use when adding devcontainer support to a project, setting
up isolated development envi
source: antigravity-awesome-skills
---

# devcontainer-setup

Creates devcontainers with Claude Code, language-specific tooling (Python/Node/Rust/Go), and persistent volumes. Use when adding devcontainer support to a project, setting up isolated development envi

## When to Use

- Use this skill when working on tasks related to devcontainer setup
- Apply best practices from antigravity-awesome-skills

## Workflow

```mermaid
flowchart TB
    start([User requests devcontainer])
    recon[1. Project Reconnaissance]
    detect[2. Detect Languages]
    generate[3. Generate Configuration]
    write[4. Write files to .devcontainer/]
    done([Done])

    start --> recon
    recon --> detect
    detect --> generate
    generate --> write
    write --> done
```

## Source

Adopted from: antigravity-awesome-skills
