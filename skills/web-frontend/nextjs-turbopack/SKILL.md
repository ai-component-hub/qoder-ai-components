---
name: 'nextjs-turbopack'
description: 'Next.js 16+ and Turbopack — incremental bundling, FS caching, dev speed,'
adopted: 2026-05-16
batch: bulk-adoption
and when to use Turbopack vs webpack.
source: everything-claude-code
tier: 3
---

# nextjs-turbopack

Next.js 16+ and Turbopack — incremental bundling, FS caching, dev speed, and when to use Turbopack vs webpack.

## When to Use

- Use this skill when working on tasks related to nextjs turbopack
- Apply best practices from everything-claude-code

## Workflow

name: nextjs-turbopack
description: Next.js 16+ and Turbopack — incremental bundling, FS caching, dev speed, and when to use Turbopack vs webpack.
origin: ECC
# Next.js and Turbopack
Next.js 16+ uses Turbopack by default for local development: an incremental bundler written in Rust that significantly speeds up dev startup and hot updates.
## When to Use
- **Turbopack (default dev)**: Use for day-to-day development. Faster cold start and HMR, especially in large apps.
- **Webpack (legacy dev)**: Use only if you hit a Turbopack bug or rely on a webpack-only plugin in dev. Disable with `--webpack

## Source

Adopted from: everything-claude-code
