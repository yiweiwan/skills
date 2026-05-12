---
name: vue-frontend
description: Use only when implementing or fixing Vue applications and components, including Composition API, Options API, Pinia, Vue Router, composables, reactive state, templates, forms, and Vue-specific behavior.
---

# Vue Frontend

## Workflow

1. Identify Vue version, router, state management, styling, and tests.
2. Follow existing component, composable, and store patterns.
3. Keep reactive state minimal and explicit.
4. Model loading, empty, error, disabled, and success states.
5. Preserve template readability.

## Rules

- Avoid accidental reactive side effects.
- Keep props, emits, and slots clear.
- Use existing UI components and directives.

## Verification

- Run typecheck, lint, tests, and build when available.
- Inspect affected UI states.
