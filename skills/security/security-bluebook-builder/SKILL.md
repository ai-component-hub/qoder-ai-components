---
name: 'security-bluebook-builder'
description: 'Build a minimal but real security policy for sensitive apps. The output'
adopted: 2026-05-16
batch: bulk-adoption
is a single, coherent Blue Book document using MUST/SHOULD/CAN language, with explicit
assumptions, scope, and security gates.
source: antigravity-awesome-skills
---

# security-bluebook-builder

"Build a minimal but real security policy for sensitive apps. The output is a single, coherent Blue Book document using MUST/SHOULD/CAN language, with explicit assumptions, scope, and security gates."

## When to Use

- Use this skill when working on tasks related to security bluebook builder
- Apply best practices from antigravity-awesome-skills

## Workflow

### 1) Gather inputs (ask only if missing)
Collect just enough context to fill the template. If the user has not provided details, ask up to 6 short questions:
- What data classes are handled (PII, PHI, financial, tokens, content)?
- What are the trust boundaries (client/server/third parties)?
- How do users authenticate (OAuth, email/password, SSO, device sessions)?
- What storage is used (DB, object storage, logs, analytics)?
- What connectors or third parties are used?
- Retention and deletion expectations (default + user-initiated)?

If the user cannot answer, proceed with safe defaults and mark TODOs.

### 2) Draft the Blue Book
Load `references/bluebook_template.md` and fill it with the provided details. Keep it concise, deterministic, and enforceable.

### 3) Enforce guardrails
- Do

## Source

Adopted from: antigravity-awesome-skills
