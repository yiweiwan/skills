---
name: graphql-api
description: Use only when designing, implementing, or modifying GraphQL schemas, queries, mutations, resolvers, dataloaders, authorization, pagination, schema evolution, and GraphQL error behavior.
---

# GraphQL API

## Workflow

1. Identify schema types, operations, clients, and authorization requirements.
2. Design fields around client needs without exposing internal persistence details.
3. Implement resolvers with batching or dataloaders to avoid N+1 queries.
4. Handle nullability, pagination, filtering, and errors consistently.
5. Evolve schema without breaking clients when possible.

## Rules

- Enforce authorization in resolvers or service layers.
- Avoid expensive unbounded nested queries.
- Deprecate fields before removing them.

## Verification

- Test queries, mutations, auth failure, nullability, and pagination.
