---
name: prompt-engineering
description: Use only when writing, revising, testing, or versioning prompts, system instructions, developer instructions, few-shot examples, output schemas, refusal behavior, and prompt regression cases.
---

# Prompt Engineering

## Workflow

1. Define the task, user input shape, desired output, constraints, and failure cases.
2. Keep instructions short, specific, and testable.
3. Use examples only when they materially improve behavior.
4. Prefer structured output when downstream code depends on format.
5. Version prompts and track changes that affect behavior.

## Rules

- Separate policy, role, task, context, examples, and output format.
- Avoid contradictory instructions.
- Do not bury critical constraints in examples only.

## Verification

- Run representative prompt tests before and after changes.
- Check ambiguity, malformed input, unsafe input, and edge cases.
