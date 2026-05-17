---
name: 'pipecat-friday-agent'
description: 'Build a low-latency, Iron Man-inspired tactical voice assistant (F.R.I.D.A.Y.)'
using Pipecat, Gemini, and OpenAI.
source: open-source (antigravity-awesome-skills)
type: autonomous_agent_skill
version: 1.0
---

# Pipecat Friday Agent

"Build a low-latency, Iron Man-inspired tactical voice assistant (F.R.I.D.A.Y.) using Pipecat, Gemini, and OpenAI."

## Autonomous Capabilities

- Autonomous operation without manual intervention
- Intelligent task planning and execution
- Self-monitoring and error recovery
- Multi-step workflow orchestration

## Use Cases

- Automated task execution
- Complex workflow management
- Intelligent decision making
- Autonomous problem solving

## Workflow

1. Initialize agent with task parameters
2. Analyze task requirements
3. Execute autonomous workflow
4. Monitor progress and handle errors
5. Report results and completion status

## Source

This autonomous agent was adopted from: `antigravity-awesome-skills/skills/pipecat-friday-agent/SKILL.md`

## Original Content

---
name: pipecat-friday-agent
description: "Build a low-latency, Iron Man-inspired tactical voice assistant (F.R.I.D.A.Y.) using Pipecat, Gemini, and OpenAI."
category: voice-agents
risk: safe
source: community
date_added: "2026-03-10"
tags: [pipecat, voice, gemini, openai, python]
tools: [pipecat]
---

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

## How It Works

### Step 1: Install Dependencies

You will need the Pipecat framework and its service providers installed:
```bash
pip install pipecat-ai[openai,google,silero] python-dotenv
```

### Step 2: Configure Environment

Create a `.env` file with your API keys:
```env
OPENAI_API_KEY=your_openai_key
GOOGLE_API_KEY=your_google_key
```

### Step 3: Run the Agent

Execute the provided Python script to start the interface:
```bash
python scripts/friday_agent.py
```

## Core Concepts

### Pipeline Architecture
The agent follows a linear pipeline: `Mic -> VAD -> STT -> LLM -> TTS -> Speaker`. This allows for granular control over each stage, unlike end-to-end speech-to-speech models.

### Google Compatibility Shim
Since Google's Gemini API has a different message format than OpenAI's standard (which Pipecat aggregators expec
