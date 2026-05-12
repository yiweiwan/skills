---
name: testing-quality
description: Use when adding, fixing, or improving tests, test strategy, coverage, mocks, fixtures, CI failures, flaky tests, unit tests, integration tests, end-to-end tests, visual tests, accessibility checks, or quality gates.
---

# Testing Quality

## Workflow

1. Identify test framework, naming conventions, fixtures, factories, mocks, and CI commands.
2. Reproduce the bug or define behavior before changing tests.
3. Add the smallest useful test at the lowest reliable level.
4. Use integration or end-to-end tests for cross-boundary behavior.
5. Keep tests deterministic, isolated, readable, and focused on stable behavior.

## Guidance

- Prefer realistic fixtures over excessive mocking.
- Mock network, time, randomness, external services, and slow boundaries deliberately.
- Test empty input, invalid input, permissions, not found, duplicates, concurrency, and partial failure.

## Verification

- Run the specific failing test first, then the nearest suite.
- Run lint, typecheck, and build when test changes touch shared code.
