---
name: database-migrations
description: Use only when creating, reviewing, or planning database migrations, schema changes, backfills, rollback plans, deploy ordering, non-null columns, unique constraints, indexes, and production data compatibility.
---

# Database Migrations

## Workflow

1. Inspect existing migrations and schema conventions.
2. Identify production data impact, locks, downtime risk, and deploy order.
3. Split risky changes into expand, backfill, contract phases.
4. Plan rollback or safe forward recovery.
5. Keep migrations deterministic and environment-safe.

## Rules

- Do not add non-null columns without defaults or backfills unless safe.
- Consider index creation cost and locking.
- Avoid destructive changes without explicit approval.

## Verification

- Run migrations locally when possible.
- Test application compatibility before and after migration.
