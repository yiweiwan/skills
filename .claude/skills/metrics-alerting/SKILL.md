---
name: metrics-alerting
description: Use only when adding or improving metrics, dashboards, alerts, SLOs, SLIs, health checks, error rates, latency metrics, saturation metrics, and production alert thresholds.
---

# Metrics Alerting

## Workflow

1. Identify the user journey, service boundary, and failure mode to monitor.
2. Choose metrics for latency, traffic, errors, saturation, freshness, or queue depth.
3. Define labels carefully and avoid unsafe high-cardinality dimensions.
4. Set alerts around user impact and actionable thresholds.
5. Add dashboard queries or runbook notes when useful.

## Rules

- Metrics should be stable, cheap, and meaningful.
- Avoid alerting on symptoms that nobody can act on.
- Distinguish warning alerts from paging alerts.

## Verification

- Confirm metrics emit in local, staging, or test paths.
- Test alert queries when possible.
