---
name: database-modeling
description: Use as a router only for broad database design work. Prefer database-migrations for schema changes, sql-querying for SQL writing, and database-performance for slow queries or index tuning.
---

# Database Modeling

## Workflow

1. Inspect schema, migrations, ORM models, naming conventions, and query patterns.
2. Route to `database-migrations`, `sql-querying`, or `database-performance` when applicable.
3. Identify entities, ownership, cardinality, lifecycle, retention, and audit needs.
4. Prefer constraints that protect durable invariants.
5. Avoid destructive changes unless explicitly requested and safely staged.

## Guidance

- Add indexes for observed query patterns, not every possible filter.
- Use parameterized queries and ORM-safe APIs.
- Check for N+1 queries, unbounded reads, missing pagination, and inefficient joins.
- Be careful with nulls, time zones, uniqueness, and soft deletes.

## Verification

- Run migrations locally when possible.
- Run affected model, repository, and integration tests.
- For risky changes, provide rollout, backfill, and rollback notes.
