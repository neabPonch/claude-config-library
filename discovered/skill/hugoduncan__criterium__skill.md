---
name: hugoduncan__criterium__skill
source: https://github.com/hugoduncan/criterium/blob/77f15121fd3b003fefbbfe7f0d2ea3defd960bcc/skills/criterium/SKILL.md
repo: hugoduncan/criterium
kind: skill
stars: 1225
last_pushed: 2026-06-10T22:10:08Z
license: unknown
score: 8
domains: [clojure, performance-engineering]
tags: [benchmarking, jvm, statistics]
curated: 2026-06-15
curated_by: config-scout
---

# hugoduncan/criterium — skill

**Why it's worth keeping:** Provides critical versioning/deprecation warnings (0.4.x vs 0.5.x) and structured patterns for 'Domain Analysis' which are essential for an agent to perform accurate performance profiling.

**Summary:** A high-density technical reference for the Criterium Clojure benchmarking library, covering statistical measurement, output viewers, and algorithmic complexity analysis.

**Source credibility:** High; reflects a well-established, widely used Clojure library with significant community adoption.

**Recency:** Current; explicitly covers the 0.5.x API specification.

**Source:** [hugoduncan/criterium/skills/criterium/SKILL.md](https://github.com/hugoduncan/criterium/blob/77f15121fd3b003fefbbfe7f0d2ea3defd960bcc/skills/criterium/SKILL.md) · 1225★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: criterium
description: Use this skill when users ask about benchmarking Clojure code, measuring performance, profiling execution time, or using the criterium library. Covers the 0.5.x API including bench macro, bench plans, viewers, domain analysis, and argument generation.
---

# Criterium

Statistically rigorous benchmarking for Clojure that accounts for JVM warmup, garbage collection, and measurement overhead.

## Overview

Criterium is the standard benchmarking library for Clojure. Unlike naive timing approaches, it provides:

- **JVM-aware measurement** - Handles JIT warmup and GC interference
- **Statistical rigor** - Bootstrap confidence intervals, outlier detection
- **Multiple output formats** - Text, structured data, interactive charts

**Library:** `org.hugoduncan/criterium`
**Current Version:** 0.5.x (alpha)
**License:** EPL-1.0

**Note:** The 0.4.x API (`criterium.core/bench`) is deprecated. Use `criterium.bench/bench` for all new code.

## Quick Start

```clojure
(require '[criterium.bench :as bench])

(bench/bench (+ 1 1))
```

Output:
```
      Elapsed Time: 2.15 ns  3σ [2.08 2.22]  min 2.07
Outliers (outliers / samples): low-severe 0 (0.0%), low-mild 0 (0
```

</details>
