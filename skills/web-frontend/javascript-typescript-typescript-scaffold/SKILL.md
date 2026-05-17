---
name: 'javascript-typescript-typescript-scaffold'
description: 'You are a TypeScript project architecture expert specializing in scaffolding production-ready Node.js and frontend applications. Generate complete project structures with modern tooling (pnpm, Vite,'
version: 1.0.0
source: antigravity-awesome-skills
tier: 4
adopted: 2026-05-16
batch: bulk-adoption
---

# javascript-typescript-typescript-scaffold

"You are a TypeScript project architecture expert specializing in scaffolding production-ready Node.js and frontend applications. Generate complete project structures with modern tooling (pnpm, Vite, 

## When to Use

- Use this skill when working on tasks related to javascript typescript typescript scaffold
- Apply best practices from antigravity-awesome-skills

## Workflow

### 1. Analyze Project Type

Determine the project type from user requirements:
- **Next.js**: Full-stack React applications, SSR/SSG, API routes
- **React + Vite**: SPA applications, component libraries
- **Node.js API**: Express/Fastify backends, microservices
- **Library**: Reusable packages, utilities, tools
- **CLI**: Command-line tools, automation scripts

### 2. Initialize Project with pnpm

```bash
# Install pnpm if needed
npm install -g pnpm

# Initialize project
mkdir project-name && cd project-name
pnpm init

# Initialize git
git init
echo "node_modules/" >> .gitignore
echo "dist/" >> .gitignore
echo ".env" >> .gitignore
```

### 3. Generate Next.js Project Structure

```bash
# Create Next.js project with TypeScript
pnpm create next-app@latest . --typescript --tailwind --app --s

## Source

Adopted from: antigravity-awesome-skills
