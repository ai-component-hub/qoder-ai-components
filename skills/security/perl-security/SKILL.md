---
name: 'perl-security'
description: 'Comprehensive Perl security covering taint mode, input validation, safe'
adopted: 2026-05-16
process execution, DBI parameterized queries, web security (XSS/SQLi/CSRF), and
perlcritic security policies.
source: everything-claude-code
tier: 2
---

# perl-security

Comprehensive Perl security covering taint mode, input validation, safe process execution, DBI parameterized queries, web security (XSS/SQLi/CSRF), and perlcritic security policies.

## When to Use

- Use this skill when working on tasks related to perl security
- Trigger when you need expertise in this domain
- Apply best practices from everything-claude-code

## Workflow

name: perl-security
description: Comprehensive Perl security covering taint mode, input validation, safe process execution, DBI parameterized queries, web security (XSS/SQLi/CSRF), and perlcritic security policies.
origin: ECC
# Perl Security Patterns
Comprehensive security guidelines for Perl applications covering input validation, injection prevention, and secure coding practices.
## When to Activate
- Handling user input in Perl applications
- Building Perl web applications (CGI, Mojolicious, Dancer2, Catalyst)
- Reviewing Perl code for security vulnerabilities
- Performing file operations with user-supplied paths
- Executing system commands from Perl
- Writing DBI database queries
## How It Works
Start with taint-aware input boundaries, then move outward: validate and untaint inputs, keep filesystem and process execution constrained, and use parameterized DBI queries everywhere. The examples below show the safe defaults this skill expects you to apply before shipping Perl code that touches user input, the shell, or the network.
## Taint Mode
Perl's taint mode (`-T`) tracks data from external sources and prevents it from being used in unsafe operations without explicit validation.
### Enabling Taint Mode
```perl
#!/usr/bin/perl -T
use v5.36;

## Source

This skill was adopted from open-source repository: everything-claude-code
Original path: perl-security
