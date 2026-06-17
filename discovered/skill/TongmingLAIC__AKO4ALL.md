---
name: TongmingLAIC__AKO4ALL
source: https://github.com/TongmingLAIC/AKO4ALL/blob/767175ef4e7d4ac37fe4e245a2fc560c8ca2c339/SKILL.md
repo: TongmingLAIC/AKO4ALL
kind: skill
stars: 287
last_pushed: 2026-05-31T08:56:09Z
license: mit
score: 9
domains: [high-performance-computing, gpu-optimization, agentic-workflows]
tags: [cuda, triton, optimization, profiling]
curated: 2026-06-14
curated_by: config-scout
---

# TongmingLAIC/AKO4ALL — skill

**Why it's worth keeping:** Uses the 'Resolved Plan' pattern to ensure path accuracy before execution and utilizes markdown files (HINTS.md) as an external memory layer for persisting user directives across turns.

**Summary:** An agentic loop designed to iteratively optimize GPU kernels through a profile-modify-benchmark cycle. It manages workspace isolation, environment friction, and persistent state tracking.

**Source credibility:** Highly credible; high star count and specific domain expertise in high-performance computing (HPC).

**Recency:** Very current; includes specific mitigations for modern environment issues like Conda path resolution.

**Source:** [TongmingLAIC/AKO4ALL/SKILL.md](https://github.com/TongmingLAIC/AKO4ALL/blob/767175ef4e7d4ac37fe4e245a2fc560c8ca2c339/SKILL.md) · 287★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: ako4all
description: Drive an agentic loop that iteratively optimizes a GPU kernel for maximum speedup. Use this skill whenever the user wants to optimize / speed up / benchmark a GPU kernel (CUDA, Triton, TileLang, C++, Python), mentions AKO / AKO4ALL / AKO4X / agentic kernel optimization, asks to "make this kernel faster", or has a kernel they want measured against a PyTorch reference. The skill handles setup, profiling (ncu), correctness checking, iteration logging, and git commits. Bootstraps a workspace in any directory the user points at.
---

# AKO4ALL — Agentic Kernel Optimization

Drive a profile → modify → benchmark → log → commit loop on a GPU kernel until it runs faster than the reference. The user provides at minimum a kernel; everything else (reference, inputs, bench script, hints) is optional.

## When this skill applies

- "optimize this kernel" / "speed up this CUDA / Triton / TileLang kernel"
- "run AKO / AKO4ALL on ..."
- "benchmark this kernel against PyTorch"
- "iterate on this kernel until it's faster"
- mentions of `ncu`, kernel profiling, GPU speedup target

Does NOT apply when:
- User wants to *write* a new kernel from scratch with no optimization
```

</details>
