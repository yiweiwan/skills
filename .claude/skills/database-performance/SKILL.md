---
name: database-performance
description: "Use only for database performance work: slow SQL, query plans, indexes, joins, pagination, N+1 queries, lock contention, table scans, partitioning, and database-specific tuning."
---

# Database Performance

## Workflow

1. Capture the slow query, parameters, row counts, and expected access pattern.
2. Inspect query plan and current indexes.
3. Identify table scans, bad joins, sort costs, lock waits, or missing pagination.
4. Add or change indexes only for real query patterns.
5. Consider migration cost and production data size.

## Rules

- Avoid indexing every column.
- Check write overhead and uniqueness semantics.
- Prefer query rewrites when they are simpler and safer than new indexes.

## Verification

- Compare query plans and timings before and after.
- Run migration and relevant repository tests.
