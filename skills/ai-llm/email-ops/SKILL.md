---
name: 'email-ops'
description: 'Evidence-first mailbox triage, drafting, send verification, and sent-mail-safe'
adopted: 2026-05-16
follow-up workflow for ECC. Use when the user wants to organize email, draft or
send through the real mail surface, or pr
source: everything-claude-code
tier: 2
---

# email-ops

Evidence-first mailbox triage, drafting, send verification, and sent-mail-safe follow-up workflow for ECC. Use when the user wants to organize email, draft or send through the real mail surface, or pr

## When to Use

- Use this skill when working on tasks related to email ops
- Trigger when you need expertise in this domain
- Apply best practices from everything-claude-code

## Workflow

### 1. Resolve the exact surface

Before acting, settle:

- which mailbox account
- which thread or recipient
- whether the task is triage, draft, reply, or send
- whether the user wants draft-only or live send

### 2. Read the thread before composing

If replying:

- read the existing thread
- identify the last outbound touch
- identify any commitments, deadlines, or unanswered questions

If creating a new outbound:

- identify warmth level
- select the correct channel and sender account
- pull `brand-voice` before drafting

### 3. Draft, then verify

For draft-only work:

- produce the final copy
- state sender, recipient, subject, and purpose

For live-send work:

- verify the exact final body first
- send through the chosen mail surface
- confirm the message landed in Sent or the equivalent sent-copy store

### 4. Report exact state

Use exact status words:

- drafted
- approval-pending
- sent
- blocked
- awaiting verification

If the send surface is blocked, preserve the draft and report the exact blocker instead of improvising a second transport without saying so.

## Source

This skill was adopted from open-source repository: everything-claude-code
Original path: email-ops
