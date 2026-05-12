---
name: mobile-app-development
description: Use when building or modifying mobile apps with React Native, Expo, Flutter, Swift, Kotlin, Android, iOS, mobile UI, navigation, native modules, device APIs, app permissions, offline state, push notifications, or app store readiness.
---

# Mobile App Development

## Workflow

1. Identify platform, framework, package manager, navigation, styling, native modules, and build tools.
2. Follow existing screen, component, state, and API patterns.
3. Design for small screens, touch targets, safe areas, keyboards, offline states, and slow networks.
4. Treat platform permissions, background behavior, and device APIs explicitly.
5. Keep Android and iOS differences visible.

## Implementation Guidance

- Use existing navigation and state management conventions.
- Avoid blocking the UI thread with heavy work.
- Handle app lifecycle, deep links, push notifications, and permission denial paths when relevant.
- Keep secrets out of app bundles.

## Verification

- Run typecheck, lint, tests, and platform build commands when available.
- Test on at least one simulator or device path when feasible.
- Check loading, error, offline, keyboard, and permission states.
