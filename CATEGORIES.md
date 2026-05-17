# Component Category System

**Version:** 2.0  
**Total Components:** 2,522  
**Categories:** 15 per component type

---

## Overview

All 2,522 AI components are organized into **15 intelligent categories** based on their domain, technology, and use case. This enables:

- **Fast Discovery** - Find relevant components by category
- **Selective Activation** - Load only what you need
- **Auto-Loading** - AI agents automatically activate categories when needed
- **Performance** - Avoid loading all 2,522 components at once

---

## Category Breakdown

### 🎨 Web Frontend (243 components)
**Focus:** UI/UX, JavaScript frameworks, frontend architecture

**Skills (193):**
- React, Vue, Angular patterns
- JavaScript/TypeScript mastery
- UI/UX design systems
- Tailwind CSS, Next.js
- Frontend performance

**Agents (33):**
- Frontend architect agents
- React/Vue/Angular specialists
- UI/UX expert agents

**Rules (17):**
- Frontend architecture standards
- Code style guidelines
- Performance rules

**Use when:** Building web interfaces, React/Vue/Angular apps, UI components

---

### 🔒 Security (79 components)
**Focus:** Security auditing, vulnerability testing, threat modeling

**Skills (65):**
- 007 (security audit)
- OWASP testing
- Threat modeling (STRIDE/PASTA)
- Penetration testing
- Encryption & auth

**Agents (4):**
- Security audit agent
- Vulnerability scanner

**Rules (10):**
- Security.md
- Authentication standards
- Encryption rules

**Use when:** Security audits, vulnerability assessments, compliance

---

### ☁️ Cloud (178 components)
**Focus:** AWS, Azure, GCP, serverless, containerization

**Skills (158):**
- AWS services (Lambda, EC2, S3)
- Azure patterns
- GCP services
- Docker, Kubernetes
- Serverless architectures

**Agents (18):**
- Cloud architect agents
- DevOps automation agents

**Rules (2):**
- Cloud security standards
- Infrastructure rules

**Use when:** Cloud deployment, serverless, containerization

---

### 🤖 AI/LLM (100 components)
**Focus:** Machine learning, LLMs, AI integration

**Skills (87):**
- LangChain patterns
- OpenAI integration
- Prompt engineering
- ML model deployment
- RAG systems

**Agents (9):**
- AI architect agents
- ML specialist agents

**Rules (4):**
- AI development standards
- Model deployment rules

**Use when:** Building AI features, LLM integration, ML models

---

### 🔄 Automation (142 components)
**Focus:** Workflows, scripting, bots, CI/CD

**Skills (134):**
- n8n workflows
- Zapier integrations
- Web scraping
- Bot development
- Task automation

**Agents (2):**
- Automation specialist agents

**Rules (6):**
- Workflow standards
- Automation best practices

**Use when:** Automating tasks, building workflows, scripting

---

### 🗄️ Database (95 components)
**Focus:** SQL, NoSQL, ORMs, database optimization

**Skills (76):**
- PostgreSQL patterns
- MongoDB optimization
- Redis caching
- Prisma ORM
- Database design

**Agents (14):**
- Database architect agents
- Query optimization agents

**Rules (5):**
- Database standards
- Migration rules

**Use when:** Database design, query optimization, migrations

---

### 🚀 DevOps (91 components)
**Focus:** CI/CD, infrastructure, deployment

**Skills (73):**
- GitHub Actions
- Jenkins pipelines
- Terraform
- Ansible
- Deployment strategies

**Agents (13):**
- DevOps engineer agents
- Infrastructure agents

**Rules (5):**
- CI/CD standards
- Infrastructure rules

**Use when:** Setting up pipelines, infrastructure as code, deployments

---

### 🧪 Testing (77 components)
**Focus:** Unit tests, integration tests, E2E testing

**Skills (64):**
- Jest patterns
- PyTest guides
- Cypress E2E
- Playwright testing
- TDD methodologies

**Agents (8):**
- Testing specialist agents
- QA automation agents

**Rules (5):**
- Testing standards
- Code coverage rules

**Use when:** Writing tests, setting up test infrastructure

---

### 🌐 Web Backend (96 components)
**Focus:** API development, backend frameworks, server architecture

**Skills (80):**
- FastAPI patterns
- Django development
- Express.js
- GraphQL architecture
- REST API design

**Agents (7):**
- Backend architect agents
- API development agents

**Rules (9):**
- API standards
- Backend architecture rules

**Use when:** Building APIs, backend services, microservices

---

### 📱 Mobile (47 components)
**Focus:** React Native, Flutter, iOS, Android

**Skills (34):**
- React Native patterns
- Flutter development
- iOS Swift guides
- Android Kotlin guides
- Expo setup

**Agents (5):**
- Mobile developer agents
- Cross-platform specialists

**Rules (8):**
- Mobile development standards
- App store guidelines

**Use when:** Building mobile apps, React Native, Flutter

---

### 📊 Data Science (36 components)
**Focus:** Data analysis, visualization, scientific computing

**Skills (27):**
- Pandas patterns
- NumPy guides
- Matplotlib visualization
- Data analysis workflows

**Agents (3):**
- Data scientist agents
- Analytics specialists

**Rules (6):**
- Data science standards
- Visualization rules

**Use when:** Data analysis, visualization, scientific computing

---

### 📝 Documentation (32 components)
**Focus:** Technical writing, docs generation, copywriting

**Skills (28):**
- README writing
- API documentation
- Blog writing
- Copywriting guides

**Agents (1):**
- Documentation specialist

**Rules (3):**
- Documentation standards
- Writing guidelines

**Use when:** Writing documentation, technical blogs, copywriting

---

### 💰 FinTech (8 components)
**Focus:** Finance, banking, payments, blockchain

**Skills (7):**
- Payment integration
- Blockchain patterns
- Trading algorithms

**Agents (1):**
- FinTech specialist

**Rules (0):**

**Use when:** Building financial apps, payment systems, crypto

---

### 🏥 Healthcare (5 components)
**Focus:** Medical, HIPAA, clinical systems

**Skills (5):**
- HIPAA compliance
- EHR integration
- FHIR standards

**Agents (0):**

**Rules (0):**

**Use when:** Healthcare apps, medical data, compliance

---

### 📦 Other (1,293 components)
**Focus:** Specialized tools, unique utilities, emerging tech

**Skills (1,021):**
- Specialized development tools
- Niche technologies
- Experimental components

**Agents (152):**
- Specialized agents
- Domain-specific tools

**Rules (120):**
- Specialized rules
- Domain-specific standards

**Use when:** Specific niche requirements not covered by main categories

---

## How to Use Categories

### 1. Browse by Category

```bash
# View all categories
cat categories.json | python3 -m json.tool | grep -A 2 '"skills"'

# List components in a category
python3 -c "
import json
with open('categories.json') as f:
    data = json.load(f)
    
for skill in data['categories']['skills']['security']['items']:
    print(skill)
"
```

### 2. Activate a Category

```bash
# Activate all security components
ln -s ~/.qoder/_backup/skills/007 ~/.qoder/skills/007
ln -s ~/.qoder/_backup/skills/web-security-testing ~/.qoder/skills/web-security-testing
ln -s ~/.qoder/_backup/agents/security-audit-agent ~/.qoder/agents/security-audit-agent
ln -s ~/.qoder/_backup/rules/Security.md ~/.qoder/rules/Security.md
```

### 3. Auto-Loading (AI Agent)

When you give the AI a task, it will automatically:
1. Identify required category
2. Activate relevant components
3. Execute the task

**Example:**
```
You: "Audit my API for security vulnerabilities"
AI:  "📦 Loading security category... Done! Starting audit..."
```

---

## Category Index

Full category index is in: `categories.json`

**Structure:**
```json
{
  "version": "2.0",
  "total_components": 2522,
  "categories": {
    "skills": {
      "security": {
        "count": 65,
        "items": ["007", "owasp-testing", ...]
      },
      "web-frontend": { ... }
    },
    "agents": { ... },
    "rules": { ... }
  }
}
```

---

## Statistics

### Component Distribution

| Category | Skills | Agents | Rules | Total | % |
|----------|--------|--------|-------|-------|---|
| Other | 1,021 | 152 | 120 | 1,293 | 51.3% |
| Web Frontend | 193 | 33 | 17 | 243 | 9.6% |
| Cloud | 158 | 18 | 2 | 178 | 7.1% |
| Automation | 134 | 2 | 6 | 142 | 5.6% |
| AI/LLM | 87 | 9 | 4 | 100 | 4.0% |
| Web Backend | 80 | 7 | 9 | 96 | 3.8% |
| Database | 76 | 14 | 5 | 95 | 3.8% |
| DevOps | 73 | 13 | 5 | 91 | 3.6% |
| Security | 65 | 4 | 10 | 79 | 3.1% |
| Testing | 64 | 8 | 5 | 77 | 3.1% |
| Mobile | 34 | 5 | 8 | 47 | 1.9% |
| Data Science | 27 | 3 | 6 | 36 | 1.4% |
| Documentation | 28 | 1 | 3 | 32 | 1.3% |
| FinTech | 7 | 1 | 0 | 8 | 0.3% |
| Healthcare | 5 | 0 | 0 | 5 | 0.2% |
| **TOTAL** | **2,052** | **270** | **200** | **2,522** | **100%** |

---

## Performance Benefits

### Without Categories
- Load all 2,522 components at startup
- Qoder IDE hangs or crashes
- 30-60 second startup time

### With Categories
- Load 0 components at startup
- Activate only needed category (50-200 components)
- Instant startup (<1 second)
- Auto-load takes 0.5-2 seconds when needed

---

## Future Enhancements

### Planned Features
1. **Smart Auto-Categorization** - ML-based category assignment
2. **Cross-Category Search** - Search across multiple categories
3. **Category Templates** - Pre-built category combinations
4. **Usage Analytics** - Track which categories are most used
5. **Category Dependencies** - Auto-load related categories

---

## Maintenance

### Adding New Components

When adding new components to the repository:

1. **Place in appropriate directory:**
   ```
   skills/my-new-skill/SKILL.md
   agents/my-new-agent/AGENT.md
   rules/my-new-rule.md
   ```

2. **Re-run categorization:**
   ```bash
   python3 scripts/organize-categories.py
   ```

3. **Verify category assignment:**
   ```bash
   cat categories.json | python3 -c "
   import json, sys
   data = json.load(sys.stdin)
   # Search for your component
   "
   ```

### Updating Categories

To modify category assignments or add new categories:

1. Edit `scripts/organize-categories.py`
2. Update `category_keywords` dictionary
3. Re-run the script

---

## Related Files

- `categories.json` - Complete category index
- `scripts/organize-categories.py` - Categorization script
- `README.md` - Main repository documentation
- `CONVERSION-COMPLETE.md` - Conversion report

---

**Last Updated:** 2026-05-17  
**Category System Version:** 2.0  
**Total Components:** 2,522
