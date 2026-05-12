---
name: frontend-implementation
description: Use as a router only for general frontend implementation when the framework is unknown or not covered by a narrower skill. Prefer react-frontend for React, vue-frontend for Vue, nextjs-frontend for Next.js, and frontend-performance for speed work.
---

# Frontend Implementation

## Workflow

1. Discover framework, package manager, scripts, routing, styling, and tests.
2. Route to `react-frontend`, `vue-frontend`, or `nextjs-frontend` when applicable.
3. Follow existing component, store, file naming, and data-fetching patterns.
4. Model loading, empty, error, disabled, optimistic, and success states.
5. Prefer semantic HTML and framework primitives.

## Guidance

- Use existing API clients and query/cache libraries before adding new ones.
- Treat server data, URL state, form state, and ephemeral UI state separately.
- Define stable dimensions for grids, boards, toolbars, tiles, and icon buttons.

## Verification

- Run formatter, linter, typecheck, tests, and build when available.
- Start the dev server for user-facing app changes and provide the local URL.
