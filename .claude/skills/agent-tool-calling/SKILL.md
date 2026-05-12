---
name: agent-tool-calling
description: Use only when designing or implementing agent workflows, tool calling, function schemas, multi-step tool plans, tool error handling, idempotent tool design, and AI agent orchestration.
---

# Agent Tool Calling

## Workflow

1. Identify agent goal, allowed tools, side effects, permissions, and stop conditions.
2. Design narrow tool schemas with clear names and typed inputs.
3. Make side-effecting tools explicit and idempotent where possible.
4. Handle tool failures, empty results, retries, and user confirmation.
5. Keep agent state and tool outputs compact and structured.

## Rules

- Do not expose broad dangerous tools without guardrails.
- Return data the model can directly use.
- Separate planning, acting, observing, and final response.

## Verification

- Test success, invalid input, missing permission, tool failure, and partial completion.
