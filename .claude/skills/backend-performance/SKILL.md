---
name: backend-performance
description: "Use only for backend performance work: API latency, throughput, concurrency, caching, serialization, network calls, queue processing, memory usage, startup time, and server-side bottlenecks."
---

# Backend Performance

## Workflow

1. Define latency, throughput, memory, or capacity target.
2. Measure the slow path with logs, profiling, traces, or benchmarks.
3. Identify bottlenecks in queries, serialization, locks, network calls, caches, or queues.
4. Optimize one bottleneck at a time.
5. Preserve correctness, authorization, and reliability.

## Common Fixes

- Add bounded caching with invalidation.
- Reduce N+1 calls and unnecessary serialization.
- Tune concurrency, batching, and queue workers.

## Verification

- Compare before and after metrics.
- Run functional and load-adjacent tests when available.
