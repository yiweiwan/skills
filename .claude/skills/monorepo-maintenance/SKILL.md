---
name: monorepo-maintenance
description: Use when working in monorepos, workspaces, package boundaries, shared libraries, dependency graphs, Nx, Turborepo, pnpm/yarn/npm workspaces, Bazel, build caching, versioning, or cross-package refactors.
---

# Monorepo Maintenance

## Workflow

1. Identify workspace manager, package graph, build system, affected commands, and ownership boundaries.
2. Locate the smallest package set affected by the requested change.
3. Preserve public package contracts unless a coordinated breaking change is requested.
4. Update shared types, generated artifacts, and package exports together.
5. Avoid broad dependency bumps unless needed.

## Guidance

- Use repo-native affected/test/build commands when available.
- Keep shared libraries general and application-specific logic in applications.
- Watch for duplicate dependencies, peer dependency drift, and circular imports.
- Update docs or examples when package APIs change.

## Verification

- Run affected lint, typecheck, test, and build commands.
- Confirm package exports and imports still resolve.
- Mention packages touched and any downstream risks.
