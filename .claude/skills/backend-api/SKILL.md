---
name: backend-api
description: Use as a router only for general backend API work when the API style is unclear. Prefer rest-api for REST endpoints, graphql-api for GraphQL, and auth-access-control for authentication or authorization.
---

# Backend API

## Workflow

1. Identify the framework, routing conventions, validation layer, error model, and tests.
2. Route to `rest-api`, `graphql-api`, or `auth-access-control` when applicable.
3. Trace the request path from route to service to persistence and response.
4. Validate external input at the boundary and normalize before business logic.
5. Preserve API contracts unless the user requested a breaking change.

## API Behavior

- Return consistent status codes, error shapes, pagination, sorting, and filtering.
- Enforce authorization near resource access, not only in UI code.
- Avoid leaking stack traces, secrets, or database details.
- Use transactions when multiple writes must succeed or fail together.

## Verification

- Add focused tests for handlers, services, validation, auth, and persistence.
- Run relevant backend tests and type checks.
- Exercise at least one success path and one failure path when practical.
