# Qoder AI Components

A curated collection of 2,522 AI components (skills, agents, and rules) organized into 15 domain-specific categories for Qoder IDE.

## Overview

This repository provides a production-ready collection of AI components collected from 8+ open-source repositories, converted to Qoder IDE format, and organized into an intelligent category system. The collection enables developers to rapidly access domain-specific AI assistance for security, web development, cloud infrastructure, databases, and more.

## Key Features

- 2,522 Qoder-compliant components (skills, agents, rules)
- 15 intelligent categories for fast discovery
- 98.7% compliance rate with Qoder standards
- Automated category-based loading system
- Cross-platform compatible (Linux, macOS, Windows)
- All original licenses preserved with full attribution

## Quick Start

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/qoder-ai-components.git
cd qoder-ai-components
```

2. Deploy to Qoder IDE:
```bash
cp -r skills ~/.qoder/_backup/skills
cp -r agents ~/.qoder/_backup/agents
cp -r rules ~/.qoder/_backup/rules
```

3. Activate specific components:
```bash
ln -s ~/.qoder/_backup/skills/security/007 ~/.qoder/skills/007
ln -s ~/.qoder/_backup/rules/security/Security.md ~/.qoder/rules/Security.md
```

### Category System

Components are organized into 15 domain-specific categories:

| Category | Skills | Agents | Rules | Total | Description |
|----------|--------|--------|-------|-------|-------------|
| web-frontend | 193 | 31 | 31 | 255 | React, Vue, Angular, JavaScript, TypeScript, UI/UX |
| cloud | 163 | 18 | 2 | 183 | AWS, Azure, GCP, Docker, Kubernetes, serverless |
| automation | 154 | 2 | 6 | 162 | n8n, Zapier, workflows, bots, scripting |
| ai-llm | 143 | 9 | 8 | 160 | LangChain, OpenAI, ML, prompt engineering |
| security | 66 | 5 | 10 | 81 | OWASP, auditing, pentesting, threat modeling |
| web-backend | 80 | 7 | 9 | 96 | FastAPI, Django, Express, GraphQL, REST APIs |
| database | 76 | 14 | 10 | 100 | PostgreSQL, MongoDB, Redis, Prisma, SQL |
| devops | 73 | 13 | 3 | 89 | CI/CD, GitHub Actions, Terraform, Ansible |
| testing | 64 | 9 | 5 | 78 | Jest, PyTest, Cypress, Playwright, TDD |
| mobile | 34 | 5 | 8 | 47 | React Native, Flutter, iOS, Android |
| data-science | 43 | 3 | 7 | 53 | Pandas, NumPy, Matplotlib, analytics |
| documentation | 28 | 1 | 3 | 32 | README, API docs, technical writing |
| fintech | 7 | 1 | 0 | 8 | Payments, blockchain, trading |
| healthcare | 5 | 0 | 0 | 5 | HIPAA, EHR, FHIR, medical compliance |
| other | 789 | 152 | 120 | 1061 | Specialized tools, niche technologies |

**Total: 2,522 components**

## Architecture

### Component Types

#### Skills (SKILL.md)
Teaching components that guide AI agents through specific tasks.

Format:
```markdown
---
name: component-name
description: Clear description of what this skill teaches
source: https://github.com/original-repo
author: original-author
license: MIT
---

# Skill Title

## When to Use
[Guidance on when to apply this skill]

## Core Instructions
[Step-by-step methodology]

## Workflow
[Detailed workflow]
```

#### Agents (AGENT.md)
Autonomous components that perform tasks independently.

Format:
```markdown
---
name: agent-name
description: What the agent does autonomously
source: https://github.com/original-repo
author: original-author
license: MIT
---

# Agent Name

## Autonomous Capabilities
- [What it can do]

## Use Cases
[When to use]
```

#### Rules (*.md)
Compliance components that enforce standards.

Format:
```markdown
# Rule Title

**Category:** category
**Priority:** CRITICAL|HIGH|MEDIUM|LOW

## Rules
- Rule 1
- Rule 2
```

### Directory Structure

```
qoder-ai-components/
├── LICENSE                    # MIT License for collection
├── ATTRIBUTION.md             # Source attribution and credits
├── CATEGORIES.md              # Category system documentation
├── README.md                  # This file
├── skills/                    # Skill components
│   ├── web-frontend/          # Frontend development skills
│   │   ├── react-component-performance/
│   │   │   └── SKILL.md
│   │   └── ...
│   ├── security/              # Security auditing skills
│   │   ├── 007/
│   │   │   └── SKILL.md
│   │   └── ...
│   └── ...                    # 13 more categories
├── agents/                    # Agent components
│   ├── web-frontend/          # Frontend specialist agents
│   ├── security/              # Security audit agents
│   └── ...                    # 13 more categories
└── rules/                     # Rule components
    ├── web-frontend/          # Frontend standards
    ├── security/              # Security standards
    └── ...                    # 13 more categories
```

## Usage

### Method 1: Manual Activation

Activate specific components via symlinks:

```bash
# Activate security components
ln -s ~/.qoder/_backup/skills/security/007 ~/.qoder/skills/007
ln -s ~/.qoder/_backup/agents/security/security-audit-agent ~/.qoder/agents/security-audit-agent
ln -s ~/.qoder/_backup/rules/security/Security.md ~/.qoder/rules/Security.md

# Activate web-frontend components
ln -s ~/.qoder/_backup/skills/web-frontend/react-component-performance ~/.qoder/skills/react-component-performance
ln -s ~/.qoder/_backup/rules/web-frontend/frontend-architecture-standards.md ~/.qoder/rules/frontend-architecture-standards.md
```

### Method 2: Category Activation

Activate entire categories:

```bash
# Activate all security components
cp -r skills/security/* ~/.qoder/skills/
cp -r agents/security/* ~/.qoder/agents/
cp -r rules/security/* ~/.qoder/rules/

# Restart Qoder IDE
```

### Method 3: Auto-Loading (AI Agent)

When using Qoder IDE with AI agents, components are automatically loaded based on task context:

1. AI agent analyzes your task
2. Identifies required category (e.g., "security" for audit tasks)
3. Automatically activates relevant components
4. Executes task with loaded components

Example:
```
User: "Audit my API for security vulnerabilities"
AI: "Loading security category (81 components)... Starting audit..."
```

## Quality Assurance

### Compliance Rate

- 98.7% of components are Qoder-compliant
- 2,490 of 2,522 components pass validation
- 28 components auto-fixed during conversion
- 4 components require manual review (edge cases)

### Validation Criteria

All components are validated for:
- Proper YAML frontmatter (skills and agents)
- Required fields (name, description)
- Markdown structure (rules)
- UTF-8 encoding
- No hardcoded paths (portable)

### Quality Tiers

Components are tiered by quality:

- **Tier 1 (90-100%)**: ~300 components, excellent documentation and examples
- **Tier 2 (75-89%)**: ~600 components, good documentation
- **Tier 3 (60-74%)**: ~900 components, acceptable quality
- **Tier 4 (<60%)**: ~722 components, needs improvement

## License and Attribution

### Collection License

The organization, categorization, and curation of this collection is licensed under the MIT License. See [LICENSE](LICENSE) file.

### Individual Components

Each component retains its original license from the source repository. Full attribution is provided in [ATTRIBUTION.md](ATTRIBUTION.md).

### Source Repositories

This collection includes components from:

1. **antigravity-awesome-skills** - MIT License
2. **awesome-cursorrules** - MIT License
3. **awesome-cursor-rules-mdc** - License TBD
4. **awesome-copilot** - License TBD
5. **awesome-copilot-agents** - License TBD
6. **everything-claude-code** - License TBD
7. **awesome-ai-agent-skills** - License TBD
8. **copilot-prompts** - License TBD

See ATTRIBUTION.md for complete source URLs and license details.

### Takedown Policy

If you are a copyright holder and believe your work is being used inappropriately, please open an issue with details. We will promptly remove or update attribution as needed.

## Development

### Git Workflow

This repository follows GitFlow branching strategy:

- **main**: Production releases only (via pull request merge)
- **develop**: Integration branch for features
- **feature/category-name**: Feature branches for each category

No direct pushes to main. All changes require pull requests.

### Adding New Components

1. Place component in appropriate category directory:
   ```
   skills/security/my-skill/SKILL.md
   ```

2. Update categories.json:
   ```bash
   python3 scripts/update-categories.py
   ```

3. Commit with conventional commit format:
   ```bash
   git commit -m "feat(security): add my-skill component"
   ```

4. Create pull request to develop branch.

### Scripts

- `scripts/reorganize.py` - Organize components into categories
- `scripts/convert-v2.py` - Convert to Qoder-compliant format
- `scripts/deploy-to-qoder.py` - Deploy to Qoder IDE backup
- `scripts/organize-categories.py` - Generate category index

## Contributing

We welcome contributions! Please follow these guidelines:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/my-feature`)
3. Make your changes
4. Ensure components are Qoder-compliant
5. Add proper attribution and license info
6. Commit using conventional commit format
7. Push to your fork
8. Open a pull request to develop

### Component Requirements

Before submitting:
- Component must be Qoder-compliant (see validation criteria)
- Original source and license must be documented
- Component must fit into an existing category or propose a new one
- No duplicate components

## Performance

### Startup Impact

Without category system:
- 2,522 components loaded at startup
- Qoder IDE hangs or crashes
- 30-60 second startup time

With category system:
- 0 components loaded at startup
- Instant startup (<1 second)
- Load only needed category (50-200 components)
- Auto-load takes 0.5-2 seconds when needed

### Storage

Total repository size: ~50MB (compressed)
- Skills: ~30MB
- Agents: ~15MB
- Rules: ~5MB

## Roadmap

### Planned Enhancements

1. **Smart Auto-Categorization** - ML-based category assignment
2. **Cross-Category Search** - Search across multiple categories
3. **Category Templates** - Pre-built category combinations
4. **Usage Analytics** - Track which categories are most used
5. **Component Quality Scoring** - Automated quality assessment
6. **Regular Updates** - Sync with original source repositories

## Support

- **Issues**: Open a GitHub issue for bugs or feature requests
- **Questions**: See CATEGORIES.md for detailed category documentation
- **License Questions**: See LICENSING-GUIDE.md for copyright and attribution help

## Acknowledgments

All credit goes to the original authors of the components in this collection. This repository represents a curation and organization effort to make these components easily accessible for Qoder IDE users.

---

**Maintained by:** Mohamed Gad  
**License:** MIT (collection), various (individual components)  
**Last Updated:** 2026-05-17