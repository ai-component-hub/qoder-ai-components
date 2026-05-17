---
name: 'adhx'
description: 'Fetch any X/Twitter post as clean LLM-friendly JSON. Converts x.com, twitter.com, or adhx.com links into structured data with full article content, author info, and engagement metrics. No scraping or'
version: 1.0.0
source: antigravity-awesome-skills
tier: 4
adopted: 2026-05-16
batch: bulk-adoption
---

# adhx

"Fetch any X/Twitter post as clean LLM-friendly JSON. Converts x.com, twitter.com, or adhx.com links into structured data with full article content, author info, and engagement metrics. No scraping or

## When to Use

- Use this skill when working on tasks related to adhx
- Apply best practices from antigravity-awesome-skills

## Workflow

When a user shares an X/Twitter link:

1. **Parse the URL** to extract `username` and `statusId` from the path segments
2. **Fetch the JSON** using curl:
```bash
curl -s "https://adhx.com/api/share/tweet/{username}/{statusId}"
```
3. **Use the structured response** to answer the user's question (summarize, analyze, extract key points, etc.)

## Source

Adopted from: antigravity-awesome-skills
