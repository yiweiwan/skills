---
name: frontend-performance
description: "Use only for frontend performance work: bundle size, Core Web Vitals, render performance, hydration, image optimization, network waterfalls, lazy loading, layout shift, and client-side responsiveness."
---

# Frontend Performance

## Workflow

1. Define the user-visible symptom and performance target.
2. Measure bundle size, network, rendering, hydration, and layout shift before changing code.
3. Identify the bottleneck: JavaScript, CSS, images, data fetching, rendering, or third-party scripts.
4. Apply the smallest effective optimization.
5. Measure again using the same method.

## Common Fixes

- Code split, lazy load, memoize carefully, reduce re-renders.
- Optimize images, fonts, caching, and critical CSS.
- Remove unused dependencies and heavy client-side work.

## Verification

- Report before and after measurements.
- Run correctness tests and inspect affected pages.
