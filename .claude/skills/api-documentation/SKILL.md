---
name: api-documentation
description: Use only when writing or improving API documentation, endpoint references, REST docs, GraphQL docs, SDK docs, authentication docs, request and response examples, error codes, rate limits, pagination, and integration guides.
---

# API Documentation

## Workflow

1. Inspect actual routes, schemas, handlers, OpenAPI specs, GraphQL schema, SDK code, or tests.
2. Identify audience: internal developer, external integrator, partner, or support engineer.
3. Document auth, base URL, endpoint or operation, parameters, request body, response, errors, limits, and examples.
4. Show realistic examples with required and optional fields.
5. Keep docs aligned with actual behavior.

## Output Pattern

- Overview and auth.
- Endpoint or operation.
- Parameters and request body.
- Response shape.
- Error cases.
- Pagination, rate limits, and idempotency.
- Example request and response.

## Verification

- Validate examples against code or schema when possible.
- Check status codes, field names, required fields, and error shapes.
