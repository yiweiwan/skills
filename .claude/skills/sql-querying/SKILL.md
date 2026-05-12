---
name: sql-querying
description: Use only when writing, reviewing, or optimizing SQL queries, joins, aggregations, CTEs, window functions, filters, reports, parameterized queries, and data correctness checks.
---

# SQL Querying

## Workflow

1. Identify tables, relationships, filters, grain, and expected result shape.
2. Confirm join keys, cardinality, null behavior, and date ranges.
3. Use parameterized queries for application code.
4. Keep reporting queries readable with CTEs when useful.
5. Validate row counts and aggregates.

## Rules

- Watch for duplicate rows from joins.
- Handle time zones and inclusive/exclusive date filters deliberately.
- Avoid unbounded reads in application paths.

## Verification

- Spot-check sample rows and totals.
- Compare against known counts or source data when available.
