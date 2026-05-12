---
name: fullstack-integration
description: Use when connecting frontend and backend behavior end to end, including API contracts, generated clients, auth sessions, cookies, CORS, file upload/download, realtime updates, form submissions, optimistic UI, and cross-layer feature implementation.
---

# Fullstack Integration

## Workflow

1. Trace UI event, request shape, API handler, service logic, persistence, response, cache update, and UI state.
2. Identify the source of truth for each field and keep contract names consistent.
3. Use existing shared types, OpenAPI specs, GraphQL schemas, generated clients, or API wrappers.
4. Design success and failure flows before coding UI.
5. Keep client validation helpful and server validation authoritative.

## Cross-Cutting Concerns

- Check cookies, CSRF, CORS, credentials, redirects, and token refresh.
- Handle time zones, locale formatting, currency, and numeric precision consistently.
- For uploads, define file size limits, accepted types, storage, and cleanup.

## Verification

- Run frontend and backend tests for the integrated path.
- Manually exercise the workflow when feasible.
- Confirm requests, status codes, payloads, cache invalidation, and UI states.
