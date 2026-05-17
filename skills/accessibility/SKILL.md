---
name: 'accessibility'
description: 'Design, implement, and audit inclusive digital products using WCAG 2.2'
adopted: 2026-05-16
Level AA
source: everything-claude-code
tier: 2
version: 1.0.0
---

# accessibility

Design, implement, and audit inclusive digital products using WCAG 2.2 Level AA

## When to Use

- Use this skill when working on tasks related to accessibility
- Trigger when you need expertise in this domain
- Apply best practices from everything-claude-code

## Workflow

name: accessibility
description: Design, implement, and audit inclusive digital products using WCAG 2.2 Level AA
  standards. Use this skill to generate semantic ARIA for Web and accessibility traits for Web and Native platforms (iOS/Android).
origin: ECC
# Accessibility (WCAG 2.2)
This skill ensures that digital interfaces are Perceivable, Operable, Understandable, and Robust (POUR) for all users, including those using screen readers, switch controls, or keyboard navigation. It focuses on the technical implementation of WCAG 2.2 success criteria.
## When to Use
- Defining UI component specifications for Web, iOS, or Android.
- Auditing existing code for accessibility barriers or compliance gaps.
- Implementing new WCAG 2.2 standards like Target Size (Minimum) and Focus Appearance.
- Mapping high-level design requirements to technical attributes (ARIA roles, traits, hints).
## Core Concepts
- **POUR Principles**: The foundation of WCAG (Perceivable, Operable, Understandable, Robust).
- **Semantic Mapping**: Using native elements over generic containers to provide built-in accessibility.
- **Accessibility Tree**: The representation of the UI that assistive technologies actually "read."
- **Focus Management**: Controlling the order and visibility of the keyboard/screen reader cursor.
- **Labeling & Hints**: Providing context through `aria-label`, `accessibilityLabel`, and `contentDescription`.
## How It Works
### Step 1: Identify the Component Role
Determine the functional purpose (e.g., Is this a button, a link, or a tab?). Use the most semantic native element available before resorting to custom roles.

## Source

This skill was adopted from open-source repository: everything-claude-code
Original path: accessibility
