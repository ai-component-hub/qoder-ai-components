---
name: 'discord-bot-architect'
description: 'Specialized skill for building production-ready Discord bots.'
adopted: 2026-05-16
batch: bulk-adoption
source: antigravity-awesome-skills
tier: 4
version: 1.0.0
---

# discord-bot-architect

Specialized skill for building production-ready Discord bots.

## When to Use

- Use this skill when working on tasks related to discord bot architect
- Apply best practices from antigravity-awesome-skills

## Workflow

1. Develop and test with guild commands (instant)
2. When ready, deploy global commands
3. Wait up to 1 hour for propagation
4. Don't deploy global commands frequently

### Frequent Gateway Disconnections

Severity: MEDIUM

Situation: Bot randomly goes offline or misses events

Symptoms:
Bot shows as offline intermittently.
Events are missed (member joins, messages).
Reconnection messages in logs.

Why this breaks:
Discord gateway requires regular heartbeats. Issues:
- Blocking operations prevent heartbeat
- Network instability
- Memory pressure causing GC pauses
- Too many guilds without sharding (2500+ requires sharding)

Recommended fix:

## Source

Adopted from: antigravity-awesome-skills
