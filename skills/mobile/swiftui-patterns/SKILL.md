---
name: 'swiftui-patterns'
description: 'SwiftUI architecture patterns, state management with @Observable, view'
adopted: 2026-05-16
composition, navigation, performance optimization, and modern iOS/macOS UI best
practices.
source: everything-claude-code
tier: 2
---

# swiftui-patterns

SwiftUI architecture patterns, state management with @Observable, view composition, navigation, performance optimization, and modern iOS/macOS UI best practices.

## When to Use

- Use this skill when working on tasks related to swiftui patterns
- Trigger when you need expertise in this domain
- Apply best practices from everything-claude-code

## Workflow

name: swiftui-patterns
description: SwiftUI architecture patterns, state management with @Observable, view composition, navigation, performance optimization, and modern iOS/macOS UI best practices.
# SwiftUI Patterns
Modern SwiftUI patterns for building declarative, performant user interfaces on Apple platforms. Covers the Observation framework, view composition, type-safe navigation, and performance optimization.
## When to Activate
- Building SwiftUI views and managing state (`@State`, `@Observable`, `@Binding`)
- Designing navigation flows with `NavigationStack`
- Structuring view models and data flow
- Optimizing rendering performance for lists and complex layouts
- Working with environment values and dependency injection in SwiftUI
## State Management
### Property Wrapper Selection
Choose the simplest wrapper that fits:
| Wrapper | Use Case |
|---------|----------|
| `@State` | View-local value types (toggles, form fields, sheet presentation) |
| `@Binding` | Two-way reference to parent's `@State` |
| `@Observable` class + `@State` | Owned model with multiple properties |
| `@Observable` class (no wrapper) | Read-only reference passed from parent |
| `@Bindable` | Two-way binding to an `@Observable` property |

## Source

This skill was adopted from open-source repository: everything-claude-code
Original path: swiftui-patterns
