---
name: ai-llm-integration
description: Use as a router only for broad AI or LLM feature work when no narrower skill clearly applies. Prefer prompt-engineering for prompts, rag-pipeline for retrieval, agent-tool-calling for tools/agents, and llm-evaluation for evals.
---

# AI LLM Integration

## Workflow

1. Identify the user goal, model provider, latency budget, cost budget, privacy constraints, and failure tolerance.
2. Identify whether the work is prompting, retrieval, tool calling, evaluation, or integration plumbing.
3. Route to a narrower skill when one applies.
4. Prefer existing SDKs, clients, tracing, retry, and secret-management patterns.
5. Design deterministic boundaries around nondeterministic model calls.

## Implementation Guidance

- Prompts: use `prompt-engineering`.
- Retrieval and embeddings: use `rag-pipeline`.
- Agents and tool calls: use `agent-tool-calling`.
- Evals and model comparison: use `llm-evaluation`.

## Verification

- Run unit tests around parsing, tool dispatch, retries, and error handling.
- Run a small eval set before changing prompts or model settings.
- Report model, temperature, token limits, fallback behavior, and known failure modes.
