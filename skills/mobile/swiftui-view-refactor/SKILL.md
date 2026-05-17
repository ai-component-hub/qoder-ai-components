---
name: 'swiftui-view-refactor'
description: 'Refactor SwiftUI views into smaller components with stable, explicit'
adopted: 2026-05-16
batch: bulk-adoption
data flow.
source: antigravity-awesome-skills
tier: 4
---

# swiftui-view-refactor

Refactor SwiftUI views into smaller components with stable, explicit data flow.

## When to Use

- Use this skill when working on tasks related to swiftui view refactor
- Apply best practices from antigravity-awesome-skills

## Workflow

1. Reorder the view to match the ordering rules.
2. Remove inline actions and side effects from `body`; move business logic into services/models and keep only thin orchestration in the view.
3. Shorten long bodies by extracting dedicated subview types; avoid rebuilding the screen out of many computed `some View` helpers.
4. Ensure stable view structure: avoid top-level `if`-based branch swapping; move conditions to localized sections/modifiers.
5. If a view model exists or is explicitly required, replace optional view models with a non-optional `@State` view model initialized in `init`.
6. Confirm Observation usage: `@State` for root `@Observable` models on iOS 17+, legacy wrappers only when the deployment target requires them.
7. Keep behavior intact: do not change layout or business logi

## Source

Adopted from: antigravity-awesome-skills
