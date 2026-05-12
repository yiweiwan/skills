---
name: browser-extension
description: Use when building or modifying Chrome, Edge, Firefox, or Safari browser extensions, including manifests, content scripts, background service workers, permissions, storage, messaging, popup UI, options pages, and WebExtension packaging.
---

# Browser Extension

## Workflow

1. Identify manifest version, target browsers, extension surfaces, permissions, and packaging scripts.
2. Separate content scripts, background logic, popup UI, options pages, and shared utilities.
3. Request the narrowest permissions that satisfy the feature.
4. Treat webpage DOM, injected content, and messages as untrusted.
5. Preserve compatibility with the repo's bundler and extension loading workflow.

## Implementation Guidance

- Use explicit message schemas between content, background, and UI contexts.
- Handle tab lifecycle, reloads, missing permissions, and unavailable pages.
- Avoid injecting remote scripts or unsafe HTML.
- Keep storage migrations safe and version-aware.

## Verification

- Build the extension and load it unpacked when possible.
- Test on a normal page, restricted page, reload, and disabled-permission path.
- Confirm manifest permissions and content script matches are minimal.
