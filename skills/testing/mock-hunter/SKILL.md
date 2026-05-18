---
name: 'mock-hunter'
description: 'Audit a live web page in five phases (catalog, click, trace, classify, report) to identify mock data, hardcoded values, LLM-generated metrics, and broken endpoints. Outputs a markdown report with REA'
version: 1.0.0
source: antigravity-awesome-skills
tier: 2
adopted: 2026-05-16
---

# mock-hunter

"Audit a live web page in five phases (catalog, click, trace, classify, report) to identify mock data, hardcoded values, LLM-generated metrics, and broken endpoints. Outputs a markdown report with REA

## When to Use

- Use this skill when working on tasks related to mock hunter
- Trigger when you need expertise in this domain
- Apply best practices from antigravity-awesome-skills

## Workflow

name: mock-hunter
description: "Audit a live web page in five phases (catalog, click, trace, classify, report) to identify mock data, hardcoded values, LLM-generated metrics, and broken endpoints. Outputs a markdown report with REAL/MOCK/LLM/HARDCODED/BROKEN/UNKNOWN verdicts per visible value."
category: testing
risk: critical
source: community
source_repo: CodeShuX/mockhunter
source_type: community
date_added: "2026-05-07"
author: CodeShuX
tags: [testing, qa, playwright, mock-detection, web-audit, ai-testing, vibe-coding, claude-code]
tools: [claude]
license: "MIT"
license_source: "https://github.com/CodeShuX/mockhunter/blob/main/LICENSE"
plugin:
  targets:
    codex: blocked
    claude: blocked
# MockHunter — Live Page Reality Check
## Overview
MockHunter is a Claude Code skill that audits a live web page and tells you, for every visible value, whether it is real, mocked, LLM-generated, hardcoded, broken, or unknown. It is built for vibe-coded apps (Lovable, Bolt, v0, Replit, AI Studio, Cursor Composer) where the UI may look complete but the data layer often is not. It uses Playwright MCP to drive a real browser, then traces each visible value through the network and DOM to its source.

## Source

This skill was adopted from open-source repository: antigravity-awesome-skills
Original path: mock-hunter
