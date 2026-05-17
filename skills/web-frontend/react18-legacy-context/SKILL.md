---
name: 'react18-legacy-context'
description: 'Provides the complete migration pattern for React legacy context API (contextTypes, childContextTypes, getChildContext) to the modern createContext API. Use this skill whenever migrating legacy conte'
version: 1.0.0
source: awesome-copilot
tier: 2
adopted: 2026-05-16
---

# react18-legacy-context

'Provides the complete migration pattern for React legacy context API (contextTypes, childContextTypes, getChildContext) to the modern createContext API. Use this skill whenever migrating legacy conte

## When to Use

- Use this skill when working on tasks related to react18 legacy context
- Trigger when you need expertise in this domain
- Apply best practices from awesome-copilot

## Workflow

name: react18-legacy-context
description: 'Provides the complete migration pattern for React legacy context API (contextTypes, childContextTypes, getChildContext) to the modern createContext API. Use this skill whenever migrating legacy context in class components - this is always a cross-file migration requiring the provider AND all consumers to be updated together. Use it before touching any contextTypes or childContextTypes code, because migrating only the provider without the consumers (or vice versa) will cause a runtime failure. Always read this skill before writing any context migration - the cross-file coordination steps here prevent the most common context migration bugs.'
# React 18 Legacy Context Migration
Legacy context (`contextTypes`, `childContextTypes`, `getChildContext`) was deprecated in React 16.3 and warns in React 18.3.1. It is **removed in React 19**.
## This Is Always a Cross-File Migration
Unlike most other migrations that touch one file at a time, context migration requires coordinating:
1. Create the context object (usually a new file)
2. Update the **provider** component
3. Update **every consumer** component
Missing any consumer leaves the app broken - it will read from the wrong context or get `undefined`.
## Migration Steps (Always Follow This Order)
```
Step 1: Find the provider (childContextTypes + getChildContext)
Step 2: Find ALL consumers (contextTypes)
Step 3: Create the context file
Step 4: Update the provider
Step 5: Update each consumer (class components → contextType, function components → useContext)
Step 6: Verify - run the app, check no legacy context warnings remain
```
## Scan Commands

## Source

This skill was adopted from open-source repository: awesome-copilot
Original path: react18-legacy-context
