---
name: 'macos-menubar-tuist-app'
description: 'Build, refactor, or review SwiftUI macOS menubar apps that use Tuist.'
adopted: 2026-05-16
batch: bulk-adoption
source: antigravity-awesome-skills
tier: 4
version: 1.0.0
---

# macos-menubar-tuist-app

Build, refactor, or review SwiftUI macOS menubar apps that use Tuist.

## When to Use

- Use this skill when working on tasks related to macos menubar tuist app
- Apply best practices from antigravity-awesome-skills

## Workflow

1. Confirm Tuist ownership
- Verify `Tuist.swift` and `Project.swift` (or workspace manifests) exist.
- Read existing run scripts before changing launch behavior.

2. Probe backend behavior before coding assumptions
- Use `curl` to verify endpoint shape, auth requirements, and pagination behavior.
- If endpoint ignores `limit/page`, implement full-list handling with local trimming in the store.

3. Implement layers from bottom to top
- Define/adjust models first.
- Add or update client request/decoding logic.
- Update store refresh, filtering, and cache policy.
- Wire views last.

4. Keep app wiring minimal
- Keep app entry focused on scene/menu wiring and dependency injection.
- Avoid embedding business logic in `App` or menu scene declarations.

5. Standardize launch ergonomics
- Ensure 

## Source

Adopted from: antigravity-awesome-skills
