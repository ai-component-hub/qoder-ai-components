---
name: 'cloudflare-workers-expert'
description: 'Expert in Cloudflare Workers and the Edge Computing ecosystem. Covers'
adopted: 2026-05-16
batch: bulk-adoption
Wrangler, KV, D1, Durable Objects, and R2 storage.
source: antigravity-awesome-skills
tier: 4
---

# cloudflare-workers-expert

"Expert in Cloudflare Workers and the Edge Computing ecosystem. Covers Wrangler, KV, D1, Durable Objects, and R2 storage."

## When to Use

- Use this skill when working on tasks related to cloudflare workers expert
- Apply best practices from antigravity-awesome-skills

## Workflow

1. **Wrangler Ecosystem**: Use `wrangler.toml` for configuration and `npx wrangler dev` for local testing.
2. **Fetch API**: Remember that Workers use the Web standard Fetch API, not Node.js globals.
3. **Bindings**: Define all bindings (KV, D1, secrets) in `wrangler.toml` and access them through the `env` parameter in the `fetch` handler.
4. **Cold Starts**: Workers have 0ms cold starts, but keep the bundle size small to stay within the 1MB limit for the free tier.
5. **Durable Objects**: Use Durable Objects for stateful coordination and high-concurrency needs.
6. **Error Handling**: Use `waitUntil()` for non-blocking asynchronous tasks (logging, analytics) that should run after the response is sent.

## Source

Adopted from: antigravity-awesome-skills
