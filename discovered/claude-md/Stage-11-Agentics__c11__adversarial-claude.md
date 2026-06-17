---
name: Stage-11-Agentics__c11__adversarial-claude
source: https://github.com/Stage-11-Agentics/c11/blob/206588057c0595273b28213b1db9c1f86da4bca5/.lattice/orchestration/c11-104/c11-104-plan-review-pack-2026-05-18T2228/adversarial-claude.md
repo: Stage-11-Agentics/c11
kind: claude-md
stars: 35
last_pushed: 2026-06-15T14:38:35Z
license: agpl-3.0
score: 10
domains: [cli-tools, systems-engineering, agents-ai]
tags: [adversarial-review, system-design, edge-case-detection]
curated: 2026-06-15
curated_by: config-scout
---

# Stage-11-Agentics/c11 — claude-md

**Why it's worth keeping:** It utilizes a 'load-bearing assumption' framework to expose non-obvious failure modes like filesystem mtime unreliability and race conditions in shell integration.

**Summary:** A high-rigor adversarial review that stress-tests technical assumptions regarding caching, concurrency, and state synchronization.

**Source credibility:** High; exhibits professional systems engineering depth typical of specialized agentic tool development.

**Recency:** Very current; features future-dated timestamps (2026) and cutting-edge agent-native multiplexing concepts.

**Source:** [Stage-11-Agentics/c11/.lattice/orchestration/c11-104/c11-104-plan-review-pack-2026-05-18T2228/adversarial-claude.md](https://github.com/Stage-11-Agentics/c11/blob/206588057c0595273b28213b1db9c1f86da4bca5/.lattice/orchestration/c11-104/c11-104-plan-review-pack-2026-05-18T2228/adversarial-claude.md) · 35★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Adversarial Plan Review — c11-104-plan (Claude)

**Plan:** C11-104 (Surface worktree + branch as derived canonical metadata chips in the sidebar)
**Reviewer mode:** Adversarial (read-only)
**Model:** Claude
**Timestamp:** 2026-05-18T22:28

---

## Executive Summary

The plan is well-shaped on the surface — clear scope, sensible decisions, a real acceptance-criteria rubric — but it leans heavily on **three load-bearing assumptions that the document never seriously stress-tests**:

1. That `(cwd, mtime(.git/HEAD))` is a sufficient cache key.
2. That shelling out to `git rev-parse` 4–10 times per OSC 7 prompt is "free" because it's off-main.
3. That a `derived` tier slots cleanly between `osc` and `heuristic` in a precedence chain that today has no real `derived` notion of its own.

Each of these is plausible. None of them are proven, and several have well-known failure modes the plan elides. The acceptance criteria are written tightly enough to feel rigorous, but at least three of them (AC4, AC10, AC11, AC18) are fudge-able as written — a delegator wanting to declare victory can pass them without the underlying property actually holding.

**Single biggest concern:** the plan treats
```

</details>
