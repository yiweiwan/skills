---
name: git-branch-commit
description: "Use only for local Git branch and commit work: checking status, staging, commit messages, branch naming, merge conflict resolution, rebasing guidance, and preserving local changes."
---

# Git Branch Commit

## Workflow

1. Run or inspect `git status` before any Git operation.
2. Preserve user changes and avoid destructive commands unless explicitly requested.
3. Keep commits focused and messages descriptive.
4. Resolve conflicts by preserving intended behavior from both sides when possible.
5. Verify working tree state before final reporting.

## Rules

- Do not reset, checkout, or clean away user changes without explicit permission.
- Do not commit unrelated changes.
- Mention files left uncommitted when relevant.

## Verification

- Check status after staging or conflict resolution.
- Run relevant tests before claiming the branch is ready.
