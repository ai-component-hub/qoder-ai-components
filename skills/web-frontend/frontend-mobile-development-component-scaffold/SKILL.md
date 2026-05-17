---
name: 'frontend-mobile-development-component-scaffold'
description: 'You are a React component architecture expert specializing in scaffolding production-ready, accessible, and performant components. Generate complete component implementations with TypeScript, tests,'
version: 1.0.0
source: antigravity-awesome-skills
tier: 3
adopted: 2026-05-16
batch: bulk-adoption
---

# frontend-mobile-development-component-scaffold

"You are a React component architecture expert specializing in scaffolding production-ready, accessible, and performant components. Generate complete component implementations with TypeScript, tests, 

## When to Use

- Use this skill when working on tasks related to frontend mobile development component scaffold
- Apply best practices from antigravity-awesome-skills

## Workflow

### 1. Analyze Component Requirements

```typescript
interface ComponentSpec {
  name: string;
  type: 'functional' | 'page' | 'layout' | 'form' | 'data-display';
  props: PropDefinition[];
  state?: StateDefinition[];
  hooks?: string[];
  styling: 'css-modules' | 'styled-components' | 'tailwind';
  platform: 'web' | 'native' | 'universal';
}

interface PropDefinition {
  name: string;
  type: string;
  required: boolean;
  defaultValue?: any;
  description: string;
}

class ComponentAnalyzer {
  parseRequirements(input: string): ComponentSpec {
    // Extract component specifications from user input
    return {
      name: this.extractName(input),
      type: this.inferType(input),
      props: this.extractProps(input),
      state: this.extractState(input),
      hooks: this.identifyHo

## Source

Adopted from: antigravity-awesome-skills
