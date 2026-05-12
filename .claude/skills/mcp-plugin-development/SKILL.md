---
name: mcp-plugin-development
description: Use when building or modifying MCP servers, Claude Code plugins, tool connectors, local integrations, plugin manifests, tool schemas, resource templates, permissions, installation docs, or AI tool extension workflows.
---

# MCP Plugin Development

## Workflow

1. Identify whether the task is an MCP server, Claude Code plugin, connector, or local tool integration.
2. Inspect manifests, schemas, tool names, permissions, transport, and authentication.
3. Keep tool inputs strongly typed and descriptions clear enough for model selection.
4. Make operations idempotent where possible and explicit when side effects occur.
5. Provide small examples for install, configuration, and first successful call.

## Design Guidance

- Prefer narrow tools with obvious names over one broad ambiguous tool.
- Return structured data that is compact and easy for the model to use.
- Avoid exposing secrets in tool output, logs, or resource contents.
- Include pagination or filtering for large resource lists.

## Verification

- Run local schema validation and at least one real tool call when possible.
- Test missing credentials, invalid input, empty result, and permission failure.
- Document required environment variables and install steps.
