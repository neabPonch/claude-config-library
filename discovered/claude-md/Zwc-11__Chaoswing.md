---
name: Zwc-11__Chaoswing
source: https://github.com/Zwc-11/Chaoswing/blob/7a4004aaf7e9c1e4b2b378ed51f1d4e3e719bb62/Claude.md
repo: Zwc-11/Chaoswing
kind: claude-md
stars: 1
last_pushed: 2026-05-27T20:04:34Z
license: mit
score: 9
domains: [machine-learning, backend]
tags: [guardrails, build-order, ml-ops]
curated: 2026-06-15
curated_by: config-scout
---

# Zwc-11/Chaoswing — claude-md

**Why it's worth keeping:** Employs 'Golden Rules' to prevent critical errors like data leakage, enforces strict separation between Django and pure PyTorch logic, and uses an ordered build sequence to control iterative progress.

**Summary:** Provides high-stakes guardrails and a sequential build roadmap to ensure architectural integrity during machine learning development.

**Source credibility:** Single star repo but contains high-density technical expertise in ML systems and software architecture.

**Recency:** Extremely current (updated 1 month ago).

**Source:** [Zwc-11/Chaoswing/Claude.md](https://github.com/Zwc-11/Chaoswing/blob/7a4004aaf7e9c1e4b2b378ed51f1d4e3e719bb62/Claude.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# ChaosWing — Claude Code Project Memory

## What we're building
Refocusing ChaosWing into a **self-supervised neural reranker for prediction-market events**:
a bi-encoder retrieves top-100 candidate markets, a fine-tuned cross-encoder reranks them,
and the relevance labels are **mined from historical implied-probability lead-lag co-movement** —
no human labeling. Evaluated with leakage-safe ranking metrics + a forecasting probe.

**The full build plan is `docs/chaoswing-rebuild-plan.md`. Read it before starting any module.**
This file is the constitution; that file is the spec.

## Golden rules (non-negotiable)
1. **No leakage, ever.** Labels and features use only data *before* the relevant cutoff/forecast timestamp.
   Splits are **temporal**, never random, and de-duplicated by `event_family`. If a change could let
   future or near-twin information into training, stop and flag it.
2. **Stay in scope.** This is one sharp ML story. Do **not** build new product surfaces, dashboards,
   or a "predict-the-future" transformer. Do not expand the cross-venue paper-trading system.
3. **Don't touch demoted surfaces.** Briefs, watchlists, agent-trust, graph-quality, paper-trading,
   and C
```

</details>
