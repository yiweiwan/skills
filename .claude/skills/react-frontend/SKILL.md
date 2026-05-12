---
name: react-frontend
description: Use only when implementing or fixing React applications and components, including hooks, state, effects, context, forms, React Router, React Query, component composition, rendering behavior, and React-specific bugs.
---

# React Frontend

## Workflow

1. Identify React version, routing, state management, styling, data fetching, and tests.
2. Follow existing component and hook patterns.
3. Keep state local unless sharing is necessary.
4. Model loading, empty, error, disabled, and success states.
5. Avoid unnecessary effects and derived state.

## Rules

- Use stable keys and avoid mutating props or state.
- Clean up subscriptions, timers, and async work.
- Keep components accessible and semantic.

## Verification

- Run typecheck, lint, tests, and build when available.
- Inspect affected UI states.
