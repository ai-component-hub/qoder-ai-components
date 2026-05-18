# Typescript React Cursorrules Prompt File

**Source:** Open-source (awesome-cursorrules/rules/typescript-react-cursorrules-prompt-file.mdc)  
**Adopted:** 2026-05-16

---

## Category

AI Coding Standards and Best Practices

## Rules

---
description: "Cursor rules for TypeScript development with React integration."
globs: **/*
alwaysApply: false
---
// TypeScript React .cursorrules

// Prefer functional components

const preferFunctionalComponents = true;

// TypeScript React best practices

const typescriptReactBestPractices = [
  "Use React.FC for functional components with props",
  "Utilize useState and useEffect hooks for state and side effects",
  "Implement proper TypeScript interfaces for props and state",
  "Use React.memo for performance optimization when needed",
  "Implement custom hooks for reusable logic",
  "Utilize TypeScript's strict mode",
];

// Folder structure

const folderStructure = `
src/
  components/
  hooks/
  pages/
  types/
  utils/
  App.tsx
  index.tsx
`;

// Additional instructions

const additionalInstructions = `
1. Use .tsx extension for files with JSX
2. Implement strict TypeScript checks
3. Utilize React.lazy and Suspense for code-splitting
4. Use type inference where possible
5. Implement error boundaries for robust error handling
6. Follow React and TypeScript best practices and naming conventions
7. Use ESLint with TypeScript and React plugins for code quality
`;


## Validation

These rules are automatically enforced by Qoder during code generation and review.

## Notes

This rule was adopted from open-source repository and converted to Qoder format.
