---
name: code-refactor
description: "Use only when refactoring existing code while preserving behavior: simplifying structure, reducing duplication, extracting functions, improving naming, clarifying data flow, and improving maintainability without changing features."
---

# Code Refactor

## Workflow

1. Characterize current behavior with tests or focused checks.
2. Identify the smallest refactor that improves readability or maintainability.
3. Preserve public interfaces unless explicitly asked to change them.
4. Avoid broad formatting churn and unrelated cleanup.
5. Run tests after each meaningful change.

## Rules

- Do not mix feature changes with refactors unless requested.
- Use existing abstractions before adding new ones.
- Keep diffs reviewable.

## Verification

- Run focused tests, type checks, and lint when available.
- Explain what behavior was preserved.
