---
name: 'springboot-security'
description: 'Spring Security best practices for authn/authz, validation, CSRF, secrets,'
adopted: 2026-05-16
headers, rate limiting, and dependency security in Java Spring Boot services.
source: everything-claude-code
tier: 2
version: 1.0.0
---

# springboot-security

Spring Security best practices for authn/authz, validation, CSRF, secrets, headers, rate limiting, and dependency security in Java Spring Boot services.

## When to Use

- Use this skill when working on tasks related to springboot security
- Trigger when you need expertise in this domain
- Apply best practices from everything-claude-code

## Workflow

name: springboot-security
description: Spring Security best practices for authn/authz, validation, CSRF, secrets, headers, rate limiting, and dependency security in Java Spring Boot services.
origin: ECC
# Spring Boot Security Review
Use when adding auth, handling input, creating endpoints, or dealing with secrets.
## When to Activate
- Adding authentication (JWT, OAuth2, session-based)
- Implementing authorization (@PreAuthorize, role-based access)
- Validating user input (Bean Validation, custom validators)
- Configuring CORS, CSRF, or security headers
- Managing secrets (Vault, environment variables)
- Adding rate limiting or brute-force protection
- Scanning dependencies for CVEs
## Authentication
- Prefer stateless JWT or opaque tokens with revocation list
- Use `httpOnly`, `Secure`, `SameSite=Strict` cookies for sessions
- Validate tokens with `OncePerRequestFilter` or resource server
```java
@Component
public class JwtAuthFilter extends OncePerRequestFilter {

## Source

This skill was adopted from open-source repository: everything-claude-code
Original path: springboot-security
