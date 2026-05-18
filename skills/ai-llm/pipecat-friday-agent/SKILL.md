---
name: 'pipecat-friday-agent'
description: 'Build a low-latency, Iron Man-inspired tactical voice assistant (F.R.I.D.A.Y.)'
adopted: 2026-05-16
using Pipecat, Gemini, and OpenAI.
source: antigravity-awesome-skills
tier: 2
version: 1.0.0
---

# pipecat-friday-agent

"Build a low-latency, Iron Man-inspired tactical voice assistant (F.R.I.D.A.Y.) using Pipecat, Gemini, and OpenAI."

## When to Use

- Use this skill when working on tasks related to pipecat friday agent
- Trigger when you need expertise in this domain
- Apply best practices from antigravity-awesome-skills

## Workflow

name: pipecat-friday-agent
description: "Build a low-latency, Iron Man-inspired tactical voice assistant (F.R.I.D.A.Y.) using Pipecat, Gemini, and OpenAI."
category: voice-agents
risk: safe
source: community
date_added: "2026-03-10"
tags: [pipecat, voice, gemini, openai, python]
tools: [pipecat]
# Pipecat Friday Agent
## Overview
This skill provides a blueprint for building **F.R.I.D.A.Y.** (Replacement Integrated Digital Assistant Youth), a local voice assistant inspired by the tactical AI from the Iron Man films. It uses the **Pipecat** framework to orchestrate a low-latency pipeline:
- **STT**: OpenAI Whisper (`whisper-1`) or `gpt-4o-transcribe`
- **LLM**: Google Gemini 2.5 Flash (via a compatibility shim)
- **TTS**: OpenAI TTS (`nova` voice)
- **Transport**: Local Audio (Hardware Mic/Speakers)
## When to Use This Skill
- Use when you want to build a real-time, conversational voice agent.
- Use when working with the Pipecat framework for pipeline-based AI.
- Use when you need to integrate multiple providers (Google and OpenAI) into a single voice loop.
- Use when building Iron Man-themed or tactical-themed voice applications.

## Source

This skill was adopted from open-source repository: antigravity-awesome-skills
Original path: pipecat-friday-agent
