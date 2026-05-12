---
name: data-engineering
description: Use when building or modifying data pipelines, ETL/ELT jobs, batch processing, streaming, data validation, warehouses, lakehouse workflows, dbt models, Airflow or Dagster jobs, ingestion, transformation, backfills, and data quality checks.
---

# Data Engineering

## Workflow

1. Identify sources, destinations, schema contracts, freshness needs, volume, and ownership.
2. Make ingestion, transformation, validation, and publishing steps explicit.
3. Prefer incremental, idempotent pipelines with replay and backfill paths.
4. Preserve lineage, timestamps, partitioning, and audit fields.
5. Separate raw, staged, transformed, and serving layers when the project uses them.

## Data Quality

- Validate row counts, uniqueness, nullability, accepted values, referential integrity, and time windows.
- Handle late-arriving data, duplicates, schema drift, and partial failures.
- Use warehouse-native operations for large data when possible.
- Keep PII handling and retention rules visible.

## Verification

- Run pipeline jobs on a small sample or dev dataset.
- Compare source and destination counts and key aggregates.
- Document backfill, rollback, and monitoring expectations.
