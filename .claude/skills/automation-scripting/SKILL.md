---
name: automation-scripting
description: Use when creating scripts, command-line tools, batch jobs, file processing utilities, data transformation scripts, local developer automation, PowerShell, Bash, Python, Node scripts, scheduled tasks, or repeatable operational workflows.
---

# Automation Scripting

## Workflow

1. Identify inputs, outputs, OS, runtime, frequency, and failure impact.
2. Prefer the repo's existing scripting language and command style.
3. Make scripts idempotent when they may be re-run.
4. Validate inputs and fail with clear messages.
5. Log progress enough for troubleshooting without exposing secrets.
6. Put destructive actions behind explicit flags, dry runs, or confirmation.

## Script Design

- Use structured parsers for JSON, CSV, XML, YAML, and archives.
- Use safe path handling and avoid shell injection.
- Stream large files when memory could matter.
- Return meaningful exit codes for CI and automation.

## Verification

- Run on a small representative sample.
- Test missing input, invalid input, and repeated execution.
- Document the command and required environment variables when useful.
