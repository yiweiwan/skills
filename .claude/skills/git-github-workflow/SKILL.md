---
name: git-github-workflow
description: Use as a router only for broad Git or GitHub workflow tasks when no narrower skill clearly applies. Prefer git-branch-commit for local branches/commits/conflicts, github-pr-issues for PRs and issues, and release-notes for changelogs or releases.
---

# Git GitHub Workflow

## Workflow

1. Identify whether the task is local Git, GitHub collaboration, release notes, or repository hygiene.
2. Route to a narrower skill whenever possible.
3. Preserve user changes and avoid destructive Git commands unless explicitly requested.
4. Keep repository-facing text clear for collaborators.
5. Maintain labels, issue templates, contribution instructions, and license expectations when relevant.

## Prefer Narrow Skills

- Local Git branch, commit, conflict, rebase: `git-branch-commit`.
- GitHub PRs, issues, labels, review replies: `github-pr-issues`.
- Changelog, version summary, migration notes: `release-notes`.

## Verification

- Run `git status` before final reporting.
- Mention uncommitted files relevant to the task.
- Do not claim tests passed unless they were run.
