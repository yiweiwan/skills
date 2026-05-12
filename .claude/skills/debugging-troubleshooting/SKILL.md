---
name: debugging-troubleshooting
description: Use when diagnosing bugs, crashes, failing commands, failing builds, runtime errors, performance issues, regressions, unexpected behavior, logs, stack traces, CI failures, dependency conflicts, or environment problems.
---

# Debugging Troubleshooting

## Workflow

1. Reproduce the issue with the smallest command, input, or user flow.
2. Capture exact errors, stack traces, versions, environment, and recent changes.
3. Form one hypothesis at a time and run a targeted check.
4. Inspect call sites, data flow, configuration, and boundary conditions before editing.
5. Fix the root cause when possible and add a regression test.

## Patterns

- Search for error messages, symbols, routes, config keys, and tests.
- Compare working and failing paths.
- Check dependency, lockfile, schema, environment, and config changes.
- For performance issues, measure before and after.

## Verification

- Re-run the original failing command or workflow.
- Run the nearest relevant tests.
- Explain cause, fix, and residual risk.
