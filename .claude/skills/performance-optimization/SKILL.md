---
name: performance-optimization
description: Use as a router only for broad performance tasks when the bottleneck is unknown. Prefer frontend-performance for frontend speed, backend-performance for server speed, and database-performance for SQL/database bottlenecks.
---

# Performance Optimization

## Workflow

1. Define the performance target and user-visible symptom.
2. Measure before changing code and identify the hot path.
3. Route to `frontend-performance`, `backend-performance`, or `database-performance` once the bottleneck is known.
4. Choose the smallest optimization that addresses the measured bottleneck.
5. Preserve correctness and avoid trading reliability for speed invisibly.

## Guidance

- Frontend symptoms: use `frontend-performance`.
- Backend symptoms: use `backend-performance`.
- Database symptoms: use `database-performance`.
- Build-only symptoms may stay here if no narrower build skill exists.

## Verification

- Report before and after measurements using the same method.
- Run correctness tests near the optimized code.
- Document remaining bottlenecks and tradeoffs.
