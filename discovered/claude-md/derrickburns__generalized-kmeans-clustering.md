---
name: derrickburns__generalized-kmeans-clustering
source: https://github.com/derrickburns/generalized-kmeans-clustering/blob/f0668a833099db2be002abaa3ed972eb8e3318f3/CLAUDE.md
repo: derrickburns/generalized-kmeans-clustering
kind: claude-md
stars: 342
last_pushed: 2026-02-14T07:59:10Z
license: apache-2.0
score: 9
domains: [data-engineering, mathematics, backend-api]
tags: [scala, spark, algorithm-implementation, prompt-engineering]
curated: 2026-06-15
curated_by: config-scout
---

# derrickburns/generalized-kmeans-clustering — claude-md

**Why it's worth keeping:** The 'Common Tasks & Prompts' section provides high-quality, ready-to-use templates for complex tasks, while the explicit instructions for updating ROADMAP.md and maintaining persistence schemas are elite patterns.

**Summary:** Provides deep technical context including strict version compatibility (Spark/Scala), mathematical constraints, and rigorous engineering standards. It effectively transforms Claude from a code generator into a project maintainer by defining roadmap maintenance workflows.

**Source credibility:** High: A well-starred (342), specialized math/Spark library with professional Scala engineering rigor.

**Recency:** Very current; accounts for modern Scala versioning and Spark evolution.

**Source:** [derrickburns/generalized-kmeans-clustering/CLAUDE.md](https://github.com/derrickburns/generalized-kmeans-clustering/blob/f0668a833099db2be002abaa3ed972eb8e3318f3/CLAUDE.md) · 342★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — Maintainer Copilot for *generalized-kmeans-clustering*

**Purpose.** This file tells Claude (or any LLM assistant) exactly how to help on this repo without wasting maintainer time. It encodes project norms, API/persistence guarantees, review rubrics, performance boundaries, and Scala engineering standards.

> TL;DR
> **Primary surface:** Spark **DataFrame/ML API** (`GeneralizedKMeans`, etc.) — **RDD API removed in v0.7.0**.
> **Versions:** Scala **2.13** (primary) / 2.12, Spark **4.0.x / 3.5.x / 3.4.x**
>   - **Spark 4.0.x**: Scala 2.13 only (2.12 dropped in Spark 4.0)
>   - **Spark 3.x**: Both Scala 2.13 and 2.12 supported
> **Math:** Bregman family — divergences include `squaredEuclidean`, `kl`, `itakuraSaito`, `l1`, `generalizedI`, `logistic`, `spherical`/`cosine`.
> **Variants:** Bisecting, X-Means, Soft/Fuzzy, Streaming, K-Medians, K-Medoids.
> **Determinism + persistence** are non-negotiable.
> **Architecture:** Modular package structure with `kernels/` and `strategies/impl/` subpackages.

---

## 0) Operating Principles (do these every time)

1. **Use the DataFrame/ML API.** Code and examples use Estimator/Model patterns and Params from this codebase. (RDD API
```

</details>
