---
name: auth-access-control
description: Use only when implementing or reviewing authentication, authorization, RBAC, ABAC, sessions, tokens, permissions, access checks, tenant isolation, login/logout flows, password reset, and privilege boundaries.
---

# Auth Access Control

## Workflow

1. Identify actors, resources, actions, trust boundaries, and tenant scope.
2. Enforce authorization server-side near resource access.
3. Keep authentication, authorization, and session management separate.
4. Handle denied, expired, missing, and malformed credentials consistently.
5. Log security-relevant events without exposing secrets.

## Rules

- Do not rely on frontend checks for access control.
- Protect cross-tenant and privilege escalation paths.
- Keep token and session lifetimes explicit.

## Verification

- Test allowed, denied, unauthenticated, expired, and cross-tenant cases.
