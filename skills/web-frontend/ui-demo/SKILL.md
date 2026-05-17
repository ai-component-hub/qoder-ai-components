---
name: 'ui-demo'
description: 'Record polished UI demo videos using Playwright. Use when the user asks'
adopted: 2026-05-16
to create a demo, walkthrough, screen recording, or tutorial video of a web application.
Produces WebM videos with visible curso
source: everything-claude-code
tier: 2
---

# ui-demo

Record polished UI demo videos using Playwright. Use when the user asks to create a demo, walkthrough, screen recording, or tutorial video of a web application. Produces WebM videos with visible curso

## When to Use

- Use this skill when working on tasks related to ui demo
- Trigger when you need expertise in this domain
- Apply best practices from everything-claude-code

## Workflow

name: ui-demo
description: Record polished UI demo videos using Playwright. Use when the user asks to create a demo, walkthrough, screen recording, or tutorial video of a web application. Produces WebM videos with visible cursor, natural pacing, and professional feel.
origin: ECC
# UI Demo Video Recorder
Record polished demo videos of web applications using Playwright's video recording with an injected cursor overlay, natural pacing, and storytelling flow.
## When to Use
- User asks for a "demo video", "screen recording", "walkthrough", or "tutorial"
- User wants to showcase a feature or workflow visually
- User needs a video for documentation, onboarding, or stakeholder presentation
## Three-Phase Process
Every demo goes through three phases: **Discover -> Rehearse -> Record**. Never skip straight to recording.
## Phase 1: Discover
Before writing any script, explore the target pages to understand what is actually there.
### Why
You cannot script what you have not seen. Fields may be `<input>` not `<textarea>`, dropdowns may be custom components not `<select>`, and comment boxes may support `@mentions` or `#tags`. Assumptions break recordings silently.
### How
Navigate to each page in the flow and dump its interactive elements:
```javascript
// Run this for each page in the flow BEFORE writing the demo script
const fields = await page.evaluate(() => {

## Source

This skill was adopted from open-source repository: everything-claude-code
Original path: ui-demo
