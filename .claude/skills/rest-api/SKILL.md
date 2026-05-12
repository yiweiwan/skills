---
name: rest-api
description: Use only when designing, implementing, or modifying REST APIs, including resources, HTTP methods, status codes, request validation, response shapes, pagination, filtering, sorting, idempotency, and REST error handling.
---

# REST API

## Workflow

1. Identify resource, action, caller, auth, and API contract.
2. Choose HTTP method and status codes according to existing repo practice.
3. Validate request body, params, query, headers, and auth context.
4. Keep response and error shapes consistent.
5. Document pagination, filtering, sorting, and idempotency when relevant.

## Rules

- Avoid leaking internal model or database details.
- Make create/update retries safe when clients may retry.
- Use consistent not-found, forbidden, conflict, and validation errors.

## Verification

- Test success, validation failure, auth failure, not found, and conflict paths.
