---
name: 'appdeploy'
description: 'Deploy web apps with backend APIs, database, and file storage. Use when'
adopted: 2026-05-16
the user asks to deploy or publish a website or web app and wants a public URL.
Uses HTTP API via curl.
source: antigravity-awesome-skills
tier: 2
---

# appdeploy

"Deploy web apps with backend APIs, database, and file storage. Use when the user asks to deploy or publish a website or web app and wants a public URL. Uses HTTP API via curl."

## When to Use

- Use this skill when working on tasks related to appdeploy
- Trigger when you need expertise in this domain
- Apply best practices from antigravity-awesome-skills

## Workflow

1. **First, get deployment instructions:**
   Call `get_deploy_instructions` to understand constraints and requirements.

2. **Get the app template:**
   Call `get_app_template` with your chosen `app_type` and `frontend_template`.

3. **Deploy the app:**
   Call `deploy_app` with your app files. For new apps, set `app_id` to `null`.

4. **Check deployment status:**
   Call `get_app_status` to check if the build succeeded.

5. **View/manage your apps:**
   Use `get_apps` to list your deployed apps.

## Source

This skill was adopted from open-source repository: antigravity-awesome-skills
Original path: appdeploy
