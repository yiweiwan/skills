---
name: security-hardening
description: Use when assessing or improving security, authentication, authorization, secrets handling, input validation, dependency vulnerabilities, web security headers, injection risks, access control, privacy, or secure coding practices.
---

# Security Hardening

## Workflow

1. Identify assets, actors, trust boundaries, data sensitivity, and entry points.
2. Trace input to storage, rendering, commands, external services, and logs.
3. Enforce authorization on the server side near data access.
4. Prefer framework-native security features and established libraries.
5. Make the smallest change that reduces actual risk.

## Checks

- Validate and encode untrusted input for SQL, HTML, shell, filesystem, URL, JSON, and logs.
- Avoid dynamic shell commands; use parameterized APIs.
- Protect secrets in environment variables or secret managers.
- Check CSRF, CORS, cookies, session lifetime, rate limits, and reset flows.

## Verification

- Add tests for authorization, validation, and abuse cases.
- Run relevant security checks if available.
- Report remaining risks clearly.
