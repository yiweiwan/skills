---
name: llm-evaluation
description: Use only when creating or improving LLM evaluations, prompt evals, regression suites, golden datasets, grading rubrics, model comparison, safety checks, and quality measurement for AI features.
---

# LLM Evaluation

## Workflow

1. Define the behavior to measure and the decision the eval supports.
2. Build a representative dataset with normal, edge, adversarial, and failure cases.
3. Choose grading: exact match, schema validation, heuristic checks, human rubric, or model judge.
4. Track model, prompt, retrieval settings, and tool versions.
5. Compare against a baseline before accepting changes.

## Rules

- Keep eval cases independent of implementation details when possible.
- Include negative cases and ambiguity cases.
- Avoid overfitting prompts to tiny eval sets.

## Verification

- Report pass rate, notable failures, and tradeoffs.
- Save regression cases for bugs found in production or testing.
