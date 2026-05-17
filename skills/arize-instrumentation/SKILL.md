---
name: 'arize-instrumentation'
description: 'Adds Arize AX tracing to an LLM application for the first time. Follows'
adopted: 2026-05-16
batch: bulk-adoption
a two-phase agent-assisted flow to analyze the codebase then implement instrumentation
after user confirmation. Use when the use
source: awesome-copilot
---

# arize-instrumentation

Adds Arize AX tracing to an LLM application for the first time. Follows a two-phase agent-assisted flow to analyze the codebase then implement instrumentation after user confirmation. Use when the use

## When to Use

- Use this skill when working on tasks related to arize instrumentation
- Apply best practices from awesome-copilot

## Workflow

1. **Check dependency manifests** to detect stack:
   - Python: `pyproject.toml`, `requirements.txt`, `setup.py`, `Pipfile`
   - TypeScript/JavaScript: `package.json`
   - Java: `pom.xml`, `build.gradle`, `build.gradle.kts`
   - Go: `go.mod`

2. **Scan import statements** in source files to confirm what is actually used.

3. **Check for existing tracing/OTel** — look for `TracerProvider`, `register()`, `opentelemetry` imports, `ARIZE_*`, `OTEL_*`, `OTLP_*` env vars, or other observability config (Datadog, Honeycomb, etc.).

4. **Identify scope** — for monorepos or multi-service projects, ask which service(s) to instrument.

### What to identify

| Item | Examples |
|------|----------|
| Language | Python, TypeScript/JavaScript, Java, Go |
| Package manager | pip/poetry/uv, npm/pnpm/yarn, m

## Source

Adopted from: awesome-copilot
