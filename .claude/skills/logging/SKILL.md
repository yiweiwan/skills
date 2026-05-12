---
name: logging
description: Use only when adding or improving application logs, structured logging, log levels, request IDs, error context, audit logs, sensitive data redaction, and log usefulness for debugging.
---

# Logging

## Workflow

1. Identify the event, audience, and debugging question the log should answer.
2. Use structured fields when the codebase supports them.
3. Include correlation IDs, user or tenant identifiers only when safe, and relevant operation context.
4. Choose the correct level: debug, info, warn, error.
5. Redact secrets and sensitive data.

## Rules

- Do not log passwords, tokens, private keys, full payment data, or sensitive prompts.
- Avoid noisy logs in hot paths.
- Include enough context to diagnose failures without stack traces everywhere.

## Verification

- Confirm logs are emitted on success and failure paths as intended.
- Check redaction and log volume risk.
