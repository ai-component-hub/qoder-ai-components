---
name: 'app-store-changelog'
description: 'Generate user-facing App Store release notes from git history since the'
adopted: 2026-05-16
batch: bulk-adoption
last tag.
source: antigravity-awesome-skills
tier: 4
---

# app-store-changelog

Generate user-facing App Store release notes from git history since the last tag.

## When to Use

- Use this skill when working on tasks related to app store changelog
- Apply best practices from antigravity-awesome-skills

## Workflow

### 1) Collect changes
- Run `scripts/collect_release_changes.sh` from the repo root to gather commits and touched files.
- If needed, pass a specific tag or ref: `scripts/collect_release_changes.sh v1.2.3 HEAD`.
- If no tags exist, the script falls back to full history.

### 2) Triage for user impact
- Scan commits and files to identify user-visible changes.
- Group changes by theme (New, Improved, Fixed) and deduplicate overlaps.
- Drop internal-only work (build scripts, refactors, dependency bumps, CI).

### 3) Draft App Store notes
- Write short, benefit-focused bullets for each user-facing change.
- Use clear verbs and plain language; avoid internal jargon.
- Prefer 5 to 10 bullets unless the user requests a different length.

### 4) Validate
- Ensure every bullet maps back to a real 

## Source

Adopted from: antigravity-awesome-skills
