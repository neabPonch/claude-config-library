---
name: mar-antaya__my-claude-skills__skill
source: https://github.com/mar-antaya/my-claude-skills/blob/a67d6982ea3ae3071b0938e4691e704cbd6fc6bb/performance-profiler/SKILL.md
repo: mar-antaya/my-claude-skills
kind: skill
stars: 145
last_pushed: 2026-03-16T00:33:41Z
license: unknown
score: 8
domains: [performance, engineering, backend, devops]
tags: [profiling, optimization, benchmarking, observability]
curated: 2026-06-15
curated_by: config-scout
---

# mar-antaya/my-claude-skills — skill

**Why it's worth keeping:** The 'Before/After' documentation template and the highly specific optimization checklists provide actionable, high-signal instructions for an agent to follow.

**Summary:** Provides a rigorous, systematic framework for identifying and fixing performance bottlenecks across multiple languages and layers.

**Source credibility:** Moderate; 145 stars indicates a useful community resource with professional-grade engineering patterns.

**Recency:** Current, utilizing modern toolchains like k6, Next.js, and Go pprof.

**Source:** [mar-antaya/my-claude-skills/performance-profiler/SKILL.md](https://github.com/mar-antaya/my-claude-skills/blob/a67d6982ea3ae3071b0938e4691e704cbd6fc6bb/performance-profiler/SKILL.md) · 145★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: "performance-profiler"
description: "Performance Profiler"
---

# Performance Profiler

**Tier:** POWERFUL  
**Category:** Engineering  
**Domain:** Performance Engineering  

---

## Overview

Systematic performance profiling for Node.js, Python, and Go applications. Identifies CPU, memory, and I/O bottlenecks; generates flamegraphs; analyzes bundle sizes; optimizes database queries; detects memory leaks; and runs load tests with k6 and Artillery. Always measures before and after.

## Core Capabilities

- **CPU profiling** — flamegraphs for Node.js, py-spy for Python, pprof for Go
- **Memory profiling** — heap snapshots, leak detection, GC pressure
- **Bundle analysis** — webpack-bundle-analyzer, Next.js bundle analyzer
- **Database optimization** — EXPLAIN ANALYZE, slow query log, N+1 detection
- **Load testing** — k6 scripts, Artillery scenarios, ramp-up patterns
- **Before/after measurement** — establish baseline, profile, optimize, verify

---

## When to Use

- App is slow and you don't know where the bottleneck is
- P99 latency exceeds SLA before a release
- Memory usage grows over time (suspected leak)
- Bundle size increased after adding dependencies
- Preparing
```

</details>
