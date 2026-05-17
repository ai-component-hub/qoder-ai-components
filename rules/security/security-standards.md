# Security Standards.Md

**Category:** Security  
**Description:** Enforce security best practices across all projects including encryption, authentication, and secret management.

---

## 🎯 Purpose

Ensure consistent security-standards.md across all projects

---

## 📏 Rules

- Never commit .env files or secrets to git
- Use AES-256-GCM for sensitive data encryption
- Implement HTTP-only cookies for sessions
- Apply Helmet security headers
- Redact secrets from all logs
- Use HTTPS/TLS for all external communications
- Implement rate limiting on all APIs

---

## ✅ Validation

- Check security-standards.md compliance in code review

---

## ❌ Anti-Patterns



---

**Based on:** Best practices and lessons learned  
**Priority:** CRITICAL
