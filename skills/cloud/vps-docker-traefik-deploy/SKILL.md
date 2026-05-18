---
name: 'vps-docker-traefik-deploy'
description: 'Plan and implement secure production deployments of Docker Compose applications'
adopted: 2026-05-16
on self-hosted VPS or cloud servers using Docker Engine, Docker Compose, Traefik,
private registries, SSH tunnels, least
source: awesome-ai-agent-skills
tier: 1
---

# vps-docker-traefik-deploy

Plan and implement secure production deployments of Docker Compose applications on self-hosted VPS or cloud servers using Docker Engine, Docker Compose, Traefik, private registries, SSH tunnels, least

## When to Use

- Use this skill when working on tasks related to vps docker traefik deploy
- Trigger when you need expertise in this domain
- Apply best practices from awesome-ai-agent-skills

## Workflow

1. Establish facts before changing anything.
2. Minimize the public network surface.
3. Baseline the host with a non-root operator account.
4. Install Docker from the official stable channel.
5. Deploy Traefik separately from the app stack.
6. Keep state outside container writable layers.
7. Deploy app images by pull, not by rebuilding on the server.
8. Validate health, backup, restore, rollback, and pruning.

## Source

This skill was adopted from open-source repository: awesome-ai-agent-skills
Original path: vps-docker-traefik-deploy
