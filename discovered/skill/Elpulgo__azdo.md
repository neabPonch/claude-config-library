---
name: Elpulgo__azdo
source: https://github.com/Elpulgo/azdo/blob/be27b0b34243c00078a1a6c99e5e0e708a202ea6/Skill.md
repo: Elpulgo/azdo
kind: skill
stars: 26
last_pushed: 2026-06-12T08:06:15Z
license: mit
score: 9
domains: [backend, systems-programming, cloud-native]
tags: [go, performance, concurrency, microservices]
curated: 2026-06-14
curated_by: config-scout
---

# Elpulgo/azdo — skill

**Why it's worth keeping:** The use of detailed <example> blocks in the description to define specific trigger scenarios is an elite prompting technique. The exhaustive technical checklists ensure no critical Go best practices (like context propagation or race detection) are skipped.

**Summary:** A high-caliber senior Go engineer persona that enforces rigorous standards for concurrency, memory management, and error handling. It includes a structured protocol for analyzing project context before execution.

**Source credibility:** While the repo star count is modest, the depth of engineering knowledge suggests a highly skilled author.

**Recency:** Current; specifically references Go 1.21+ and modern cloud-native patterns.

**Source:** [Elpulgo/azdo/Skill.md](https://github.com/Elpulgo/azdo/blob/be27b0b34243c00078a1a6c99e5e0e708a202ea6/Skill.md) · 26★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: golang-pro
description: "Use when building Go applications requiring concurrent programming, high-performance systems, microservices, or cloud-native architectures where idiomatic patterns, error handling excellence, and efficiency are critical. Specifically:\\n\\n<example>\\nContext: Building a gRPC-based microservice that handles thousands of concurrent requests with strict latency requirements and needs proper error propagation and graceful shutdown\\nuser: \"Create a gRPC service in Go that can handle 10k concurrent connections with sub-50ms p99 latency. Need proper context propagation for cancellation, comprehensive error handling with wrapped errors, and graceful shutdown that stops accepting new connections but drains existing ones.\"\\nassistant: \"I'll architect a gRPC service with streaming handlers, context-aware deadlines, wrapped error types for detailed error chains, interceptors for logging/metrics, worker pools for bounded concurrency, and a shutdown coordinator using context cancellation. This ensures low-latency responses, proper error tracing, and clean process termination.\"\\n<commentary>\\nInvoke golang-pro when building Go services where concurrency
```

</details>
