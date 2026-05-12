---
name: code-review
description: Use only when reviewing code or pull requests for bugs, regressions, security risks, data loss, missing tests, maintainability concerns, and behavioral issues. Do not use for behavior-preserving refactoring work.
---

# Code Review

## Workflow

1. Understand intent, diff, affected contracts, and runtime paths.
2. Prioritize correctness, security, data loss, regressions, missing tests, and operational risk.
3. Report findings first, ordered by severity, with file and line references.
4. Keep summaries brief and secondary.
5. If no issues are found, say so and note residual test gaps.

## Review Focus

- Broken behavior, edge cases, concurrency, permissions, validation, and error handling.
- API contract drift and migration risks.
- Test coverage for changed behavior.

## Verification

- Reference exact files and lines.
- Do not rewrite code unless the user asks for a fix.
