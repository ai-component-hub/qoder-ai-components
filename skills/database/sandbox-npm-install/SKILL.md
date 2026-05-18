---
name: 'sandbox-npm-install'
description: 'Install npm packages in a Docker sandbox environment. Use this skill whenever you need to install, reinstall, or update node_modules inside a container where the workspace is mounted via virtiofs. Na'
version: 1.0.0
source: awesome-copilot
tier: 3
adopted: 2026-05-16
batch: bulk-adoption
---

# sandbox-npm-install

'Install npm packages in a Docker sandbox environment. Use this skill whenever you need to install, reinstall, or update node_modules inside a container where the workspace is mounted via virtiofs. Na

## When to Use

- Use this skill when working on tasks related to sandbox npm install
- Apply best practices from awesome-copilot

## Workflow

name: sandbox-npm-install
description: 'Install npm packages in a Docker sandbox environment. Use this skill whenever you need to install, reinstall, or update node_modules inside a container where the workspace is mounted via virtiofs. Native binaries (esbuild, lightningcss, rollup) crash on virtiofs, so packages must be installed on the local ext4 filesystem and symlinked back.'
# Sandbox npm Install
## When to Use This Skill
Use this skill whenever:
- You need to install npm packages for the first time in a new sandbox session
- `package.json` or `package-lock.json` has changed and you need

## Source

Adopted from: awesome-copilot
