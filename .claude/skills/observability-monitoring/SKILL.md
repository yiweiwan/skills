---
name: observability-monitoring
description: Use as a router only for broad observability work when the requested signal is unclear. Prefer logging for logs, metrics-alerting for metrics/dashboards/alerts, and tracing for distributed traces.
---

# Observability Monitoring

## Workflow

1. Identify service boundaries, critical user journeys, failure modes, and existing telemetry tools.
2. Determine whether the task needs logs, metrics, alerts, traces, or a mix.
3. Route to a narrower skill whenever possible.
4. Keep telemetry useful without exposing secrets or sensitive data.
5. Define monitoring around user impact.

## Guidance

- Logs: use `logging`.
- Metrics, dashboards, health checks, SLOs, alerts: use `metrics-alerting`.
- Distributed traces and span instrumentation: use `tracing`.

## Verification

- Confirm telemetry is emitted in local or staging environments.
- Test alert conditions or dashboard queries when possible.
- Document runbook notes for new alerts.
