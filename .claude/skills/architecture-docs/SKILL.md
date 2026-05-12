---
name: architecture-docs
description: Use only when writing or improving architecture documentation, system design notes, ADRs, component diagrams, service boundaries, data flow descriptions, tradeoff analysis, design decisions, constraints, and migration architecture.
---

# Architecture Docs

## Workflow

1. Identify system scope, audience, decision context, constraints, and current state.
2. Inspect code, configs, schemas, diagrams, and deployment topology when available.
3. Document components, responsibilities, data flow, dependencies, failure modes, and tradeoffs.
4. Separate current architecture, proposed architecture, decisions, and open questions.
5. Keep diagrams or textual diagrams consistent with the implementation.

## Output Patterns

- Architecture overview.
- ADR: context, decision, options, consequences.
- Data flow.
- Service boundary map.
- Migration architecture.

## Verification

- Check names, services, queues, databases, protocols, and ownership.
- Mark assumptions and stale areas.
