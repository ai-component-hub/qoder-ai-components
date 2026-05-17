---
name: 'address-github-comments'
description: 'Use when you need to address review or issue comments on an open GitHub'
adopted: 2026-05-16
batch: bulk-adoption
Pull Request using the gh CLI.
source: antigravity-awesome-skills
tier: 4
---

# address-github-comments

"Use when you need to address review or issue comments on an open GitHub Pull Request using the gh CLI."

## When to Use

- Use this skill when working on tasks related to address github comments
- Apply best practices from antigravity-awesome-skills

## Workflow

### 1. Inspect Comments

Fetch the comments for the current branch's PR.

```bash
gh pr view --comments
```

Or use a custom script if available to list threads.

### 2. Categorize and Plan

- List the comments and review threads.
- Propose a fix for each.
- **Wait for user confirmation** on which comments to address first if there are many.

### 3. Apply Fixes

Apply the code changes for the selected comments.

### 4. Respond to Comments

Once fixed, respond to the threads as resolved.

```bash
gh pr comment <PR_NUMBER> --body "Addressed in latest commit."
```

## Source

Adopted from: antigravity-awesome-skills
