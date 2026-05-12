---
name: code-review-refactor
description: Use as a router only when the user asks broadly about code quality and it is unclear whether they need review or refactoring. Prefer code-review for PR/code review findings and code-refactor for behavior-preserving refactoring.
---

# Code Review Refactor

## Workflow

1. Determine whether the task is review, refactor, or both.
2. Use `code-review` for finding issues in a diff or PR.
3. Use `code-refactor` for behavior-preserving code changes.
4. If both are requested, review first, then refactor only after the requested scope is clear.

## Boundaries

- Do not mix feature work into refactors.
- Do not edit code during a review unless asked.
- Keep findings and changes separate in the final response.
