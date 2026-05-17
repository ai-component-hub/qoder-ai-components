# Cursor Rules Docs

**Source:** Open-source (awesome-cursor-rules-mdc/cursor-rules-docs.md)  
**Adopted:** 2026-05-16

---

## Category

AI Coding Standards and Best Practices

## Rules

export const meta = {
  title: "Rules",
  description: "Configure persistent instructions with Project, Team, and User Rules, plus AGENTS.md. Learn best practices for effective coding guidelines."
};

# Rules

Rules provide system-level instructions to Agent. They bundle prompts, scripts, and more together, making it easy to manage and share workflows across your team.

Cursor supports four types of rules:

<CardGroup cols={2}>
  <Card title="Project Rules" icon="folder-tree">
    Stored in `.cursor/rules`, version-controlled and scoped to your codebase.
  </Card>
  <Card title="User Rules" icon="user">
    Global to your Cursor environment. Used by Agent (Chat).
  </Card>
  <Card title="Team Rules" icon="users">
    Team-wide rules managed from the dashboard. Available on Team and [Enterprise](/docs/enterprise) plans.
  </Card>
  <Card title="AGENTS.md" icon="bot">
    Agent instructions in markdown format. Simple alternative to
    `.cursor/rules`.
  </Card>
</CardGroup>

## How rules work

Large language models don't retain memory between completions. Rules provide persistent, reusable context at the prompt level.

When applied, rule contents are included at the start of the model context. This gives the AI consistent guidance for generating code, interpreting edits, or helping with workflows.

<Image
  height={674}
  width={1198}
  lightSrc="/docs-static/images/context/rules/rules-applied.png"
  alt="Rule applied in context with chat"
/>



## Project rules

Project rules live in `.cursor/rules`. Each rule is a folder containing a `RULE.md` file and is version-controlled. They are scoped using path patterns, invoked manually, or included based on relevance.

Use project rules to:

- Encode domain-specific knowledge about your codebase
- Automate project-specific workflows or templates
- Standardize style or architecture decisions

### Rule folder structure

Each rule folder can contain:

- **`RULE.md`** — The main rule file with frontmatter metadata and instructions
- **Scripts and prompts** — Additional files referenced by the rule

```bash
.cursor/rules/
  my-rule/
    RULE.md           # Main rule file
    scripts/          # Helper scripts (optional)
```

### Rule anatomy

Each rule is a folder containing a `RULE.md` file with frontmatter metadata and content. Control how rules are applied from the type dropdown which changes properties `description`, `globs`, `alwaysApply`.

| <span className="no-wrap">Rule Type</span>                    | Description                                                                      |
| :--------------------------------------------------------- | :------------------------------------------------------------------------------- |
| <span className="no-wrap">`Always Apply`</span>             | Apply to every chat session                                                     |
| <span className="no-wrap">`Apply Intelligently`</span>      | When Agent decides it's relevant based on description                           |
| <span className="no-wrap">`Apply to Specific Files`</span> | When file matches a specified pattern                                           |
| <span className="no-wrap">`Apply Manually`</span>           | When @-mentioned in chat (e.g., `@my-rule`)                                     |

```md
---
globs:
alwaysApply: false
---

- Use our internal RPC pattern when defining services
- Always use snake_case for service names.

@service-template.ts
```

### Creating a rule

Create rules using the `New Cursor Rule` command or going to `Cursor Settings > Rules, Commands`. This creates a new rule folder in `.cursor/rules`. From settings you can see all rules and their status.

<Image
  height={3334}
  width={6016}
  lightSrc="/docs-static/images/context/rules/rule-settings.png"
  alt="Comparison of concise vs long rules"
/>

## Best practices

Good rules are focused, actionable, and scoped.

- Keep rules under 500 lines
- Split large rules into multiple, composable rules
- Provide concrete examples or referenced files
- Avoid vague guidance. Write rules like clear internal docs
- Reuse rules when repeating prompts in chat

## RULE.md file format

The `RULE.md` file is a markdown file with frontmatter metadata and content. The frontmatter metadata is used to control how the rule is applied. The content is the rule itself.

```markdown
---
description: "This rule provides standards for frontend components and API validation"
alwaysApply: false
---

...rest of the rule content
```

If alwaysApply is true, the rule will be applied to every chat session. Otherwise, the description of the rule will be presented to the Cursor Agent to decide if it should be applied.

## Examples

<AccordionGroup>
  <Accordion title="Standards for frontend components and API validation">
    This rule provides standards for frontend components:

    When working in components directory:
    - Always use Tailwind for styling
    - Use Framer Motion for animations
    - Follow compo...

## Validation

These rules are automatically enforced by Qoder during code generation and review.

## Notes

This rule was adopted from open-source repository and converted to Qoder format.
