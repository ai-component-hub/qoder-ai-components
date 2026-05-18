---
name: 'nuxt4-patterns'
description: 'Nuxt 4 app patterns for hydration safety, performance, route rules, lazy'
adopted: 2026-05-16
loading, and SSR-safe data fetching with useFetch and useAsyncData.
source: everything-claude-code
tier: 2
version: 1.0.0
---

# nuxt4-patterns

Nuxt 4 app patterns for hydration safety, performance, route rules, lazy loading, and SSR-safe data fetching with useFetch and useAsyncData.

## When to Use

- Use this skill when working on tasks related to nuxt4 patterns
- Trigger when you need expertise in this domain
- Apply best practices from everything-claude-code

## Workflow

name: nuxt4-patterns
description: Nuxt 4 app patterns for hydration safety, performance, route rules, lazy loading, and SSR-safe data fetching with useFetch and useAsyncData.
origin: ECC
# Nuxt 4 Patterns
Use when building or debugging Nuxt 4 apps with SSR, hybrid rendering, route rules, or page-level data fetching.
## When to Activate
- Hydration mismatches between server HTML and client state
- Route-level rendering decisions such as prerender, SWR, ISR, or client-only sections
- Performance work around lazy loading, lazy hydration, or payload size
- Page or component data fetching with `useFetch`, `useAsyncData`, or `$fetch`
- Nuxt routing issues tied to route params, middleware, or SSR/client differences
## Hydration Safety
- Keep the first render deterministic. Do not put `Date.now()`, `Math.random()`, browser-only APIs, or storage reads directly into SSR-rendered template state.
- Move browser-only logic behind `onMounted()`, `import.meta.client`, `ClientOnly`, or a `.client.vue` component when the server cannot produce the same markup.
- Use Nuxt's `useRoute()` composable, not the one from `vue-router`.
- Do not use `route.fullPath` to drive SSR-rendered markup. URL fragments are client-only, which can create hydration mismatches.
- Treat `ssr: false` as an escape hatch for truly browser-only areas, not a default fix for mismatches.
## Data Fetching
- Prefer `await useFetch()` for SSR-safe API reads in pages and components. It forwards server-fetched data into the Nuxt payload and avoids a second fetch on hydration.
- Use `useAsyncData()` when the fetcher is not a simple `$fetch()` call, when you need a custom key, or when you are composing multiple async sources.

## Source

This skill was adopted from open-source repository: everything-claude-code
Original path: nuxt4-patterns
