---
name: 'x-api'
description: 'X/Twitter API integration for posting tweets, threads, reading timelines,'
adopted: 2026-05-16
search, and analytics. Covers OAuth auth patterns, rate limits, and platform-native
content posting. Use when the user wants t
source: everything-claude-code
tier: 2
---

# x-api

X/Twitter API integration for posting tweets, threads, reading timelines, search, and analytics. Covers OAuth auth patterns, rate limits, and platform-native content posting. Use when the user wants t

## When to Use

- Use this skill when working on tasks related to x api
- Trigger when you need expertise in this domain
- Apply best practices from everything-claude-code

## Workflow

name: x-api
description: X/Twitter API integration for posting tweets, threads, reading timelines, search, and analytics. Covers OAuth auth patterns, rate limits, and platform-native content posting. Use when the user wants to interact with X programmatically.
origin: ECC
# X API
> **Drift-prone skill.** X API endpoints, access tiers, quotas, and write
> permissions change frequently. Verify current developer docs and account
> access before quoting rate limits or implementing a posting/search flow.
Programmatic interaction with X (Twitter) for posting, reading, searching, and analytics.
## When to Activate
- User wants to post tweets or threads programmatically
- Reading timeline, mentions, or user data from X
- Searching X for content, trends, or conversations
- Building X integrations or bots
- Analytics and engagement tracking
- User says "post to X", "tweet", "X API", or "Twitter API"
## Authentication
### OAuth 2.0 Bearer Token (App-Only)
Best for: read-heavy operations, search, public data.
```bash
# Environment setup

## Source

This skill was adopted from open-source repository: everything-claude-code
Original path: x-api
