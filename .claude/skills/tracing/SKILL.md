---
name: tracing
description: Use only when adding or improving distributed tracing, spans, trace context propagation, request correlation, OpenTelemetry instrumentation, dependency timing, and trace-based production diagnostics.
---

# Tracing

## Workflow

1. Identify request path, service boundaries, dependencies, and missing visibility.
2. Add spans around meaningful operations, not every tiny function.
3. Propagate trace context across HTTP, queues, jobs, and async boundaries.
4. Add attributes that help diagnose latency and failures without leaking secrets.
5. Connect traces to logs and metrics when possible.

## Rules

- Avoid high-cardinality or sensitive span attributes.
- Keep span names stable and readable.
- Record errors consistently.

## Verification

- Confirm traces appear in the configured backend.
- Check parent-child relationships and important dependency timings.
