---
name: 'speckit-updater'
description: 'speckit-updater'
adopted: 2026-05-16
batch: bulk-adoption
source: antigravity-awesome-skills
tier: 4
version: 1.0.0
---

# speckit-updater

SpecKit Safe Update

## When to Use

- Use this skill when working on tasks related to speckit updater
- Apply best practices from antigravity-awesome-skills

## Workflow

1. Prerequisites validation (critical checks must pass, warnings allow continuation)
2. Manifest loading/creation (safe default: assume all files customized if no manifest)
3. GitHub API query for target version
4. File state analysis (6 actions: add/remove/merge/preserve/update/skip)
5. User confirmation with change preview
6. Backup creation (timestamped, excludes backups directory)
7. Selective file updates (fail-fast with automatic rollback)
8. Conflict resolution (Flow A: one-at-a-time, VSCode merge editor)
9. Manifest update (version, file hashes, customization flags)
10. Backup cleanup (keep 5 most recent, requires confirmation)
11. Detailed summary display

## Source

Adopted from: antigravity-awesome-skills
