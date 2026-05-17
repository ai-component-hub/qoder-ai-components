---
name: 'data-scraper-agent'
description: 'Build a fully automated AI-powered data collection agent for any public'
adopted: 2026-05-16
batch: bulk-adoption
source — job boards, prices, news, GitHub, sports, anything. Scrapes on a schedule,
enriches data with a free LLM (Gemini Flash)
source: everything-claude-code
---

# data-scraper-agent

Build a fully automated AI-powered data collection agent for any public source — job boards, prices, news, GitHub, sports, anything. Scrapes on a schedule, enriches data with a free LLM (Gemini Flash)

## When to Use

- Use this skill when working on tasks related to data scraper agent
- Apply best practices from everything-claude-code

## Workflow

### Step 1: Understand the Goal

Ask the user:

1. **What to collect:** "What data source? URL / API / RSS / public endpoint?"
2. **What to extract:** "What fields matter? Title, price, URL, date, score?"
3. **How to store:** "Where should results go? Notion, Google Sheets, Supabase, or local file?"
4. **How to enrich:** "Do you want AI to score, summarise, classify, or match each item?"
5. **Frequency:** "How often should it run? Every hour, daily, weekly?"

Common examples to prompt:
- Job boards → score relevance to resume
- Product prices → alert on drops
- GitHub repos → summarise new releases
- News feeds → classify by topic + sentiment
- Sports results → extract stats to tracker
- Events calendar → filter by interest

---

### Step 2: Design the Agent Architecture

Generate this dir

## Source

Adopted from: everything-claude-code
