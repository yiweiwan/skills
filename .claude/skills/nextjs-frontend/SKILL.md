---
name: nextjs-frontend
description: Use only when implementing or fixing Next.js applications, including App Router, Pages Router, server components, client components, route handlers, metadata, data fetching, caching, server actions, and Next.js deployment behavior.
---

# Next.js Frontend

## Workflow

1. Identify Next.js version, App Router or Pages Router, rendering mode, and deployment target.
2. Decide server component versus client component deliberately.
3. Keep data fetching, caching, revalidation, and mutations explicit.
4. Preserve route structure and metadata conventions.
5. Handle loading, error, not-found, and redirect states.

## Rules

- Do not move code to the client unless interactivity requires it.
- Watch for server-only secrets crossing into client bundles.
- Keep route handlers and UI components separate.

## Verification

- Run lint, typecheck, tests, and build.
- Check server/client boundary and affected routes.
