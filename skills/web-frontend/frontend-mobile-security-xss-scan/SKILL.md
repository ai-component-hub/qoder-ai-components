---
name: 'frontend-mobile-security-xss-scan'
description: 'You are a frontend security specialist focusing on Cross-Site Scripting (XSS) vulnerability detection and prevention. Analyze React, Vue, Angular, and vanilla JavaScript code to identify injection po'
version: 1.0.0
source: antigravity-awesome-skills
tier: 4
adopted: 2026-05-16
batch: bulk-adoption
---

# frontend-mobile-security-xss-scan

"You are a frontend security specialist focusing on Cross-Site Scripting (XSS) vulnerability detection and prevention. Analyze React, Vue, Angular, and vanilla JavaScript code to identify injection po

## When to Use

- Use this skill when working on tasks related to frontend mobile security xss scan
- Apply best practices from antigravity-awesome-skills

## Workflow

### 1. XSS Vulnerability Detection

Scan codebase for XSS vulnerabilities using static analysis:

```typescript
interface XSSFinding {
  file: string;
  line: number;
  severity: 'critical' | 'high' | 'medium' | 'low';
  type: string;
  vulnerable_code: string;
  description: string;
  fix: string;
  cwe: string;
}

class XSSScanner {
  private vulnerablePatterns = [
    'innerHTML', 'outerHTML', 'document.write',
    'insertAdjacentHTML', 'location.href', 'window.open'
  ];

  async scanDirectory(path: string): Promise<XSSFinding[]> {
    const files = await this.findJavaScriptFiles(path);
    const findings: XSSFinding[] = [];

    for (const file of files) {
      const content = await fs.readFile(file, 'utf-8');
      findings.push(...this.scanFile(file, content));
    }

    return fi

## Source

Adopted from: antigravity-awesome-skills
