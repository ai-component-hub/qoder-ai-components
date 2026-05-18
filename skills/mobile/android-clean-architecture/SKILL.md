---
name: 'android-clean-architecture'
description: 'Clean Architecture patterns for Android and Kotlin Multiplatform projects'
adopted: 2026-05-16
— module structure, dependency rules, UseCases, Repositories, and data layer patterns.
source: everything-claude-code
tier: 2
version: 1.0.0
---

# android-clean-architecture

Clean Architecture patterns for Android and Kotlin Multiplatform projects — module structure, dependency rules, UseCases, Repositories, and data layer patterns.

## When to Use

- Use this skill when working on tasks related to android clean architecture
- Trigger when you need expertise in this domain
- Apply best practices from everything-claude-code

## Workflow

name: android-clean-architecture
description: Clean Architecture patterns for Android and Kotlin Multiplatform projects — module structure, dependency rules, UseCases, Repositories, and data layer patterns.
origin: ECC
# Android Clean Architecture
Clean Architecture patterns for Android and KMP projects. Covers module boundaries, dependency inversion, UseCase/Repository patterns, and data layer design with Room, SQLDelight, and Ktor.
## When to Activate
- Structuring Android or KMP project modules
- Implementing UseCases, Repositories, or DataSources
- Designing data flow between layers (domain, data, presentation)
- Setting up dependency injection with Koin or Hilt
- Working with Room, SQLDelight, or Ktor in a layered architecture
## Module Structure
### Recommended Layout
```
project/
├── app/                  # Android entry point, DI wiring, Application class
├── core/                 # Shared utilities, base classes, error types
├── domain/               # UseCases, domain models, repository interfaces (pure Kotlin)
├── data/                 # Repository implementations, DataSources, DB, network
├── presentation/         # Screens, ViewModels, UI models, navigation

## Source

This skill was adopted from open-source repository: everything-claude-code
Original path: android-clean-architecture
