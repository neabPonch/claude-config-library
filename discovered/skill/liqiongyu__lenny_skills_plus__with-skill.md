---
name: liqiongyu__lenny_skills_plus__with-skill
source: https://github.com/liqiongyu/lenny_skills_plus/blob/df4fa3412a9252d86c92f32351ba997e31667790/skills/platform-infrastructure/eval/with_skill.md
repo: liqiongyu/lenny_skills_plus
kind: skill
stars: 52
last_pushed: 2026-05-21T14:06:30Z
license: apache-2.0
score: 9
domains: [backend, architecture, infrastructure, platform-engineering]
tags: [architectural-blueprints, migration-strategy, platformization]
curated: 2026-06-16
curated_by: config-scout
---

# liqiongyu/lenny_skills_plus — skill

**Why it's worth keeping:** Uses high-fidelity context snapshots, detailed 'current vs. proposed' capability tables, and explicit non-goals to prevent agent scope creep during large refactors.

**Summary:** A highly structured strategic blueprint for transitioning a fragmented codebase into shared platform services.

**Source credibility:** Moderate; based on specialized RefoundAI skills with decent social proof (52 stars).

**Recency:** Current/Forward-looking; uses a 2026 timestamp suggesting it is designed for modern, complex enterprise contexts.

**Source:** [liqiongyu/lenny_skills_plus/skills/platform-infrastructure/eval/with_skill.md](https://github.com/liqiongyu/lenny_skills_plus/blob/df4fa3412a9252d86c92f32351ba997e31667790/skills/platform-infrastructure/eval/with_skill.md) · 52★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Platform & Infrastructure Improvement Pack

**Company:** B2B Analytics SaaS (Series B, 50 engineers)
**Date:** 2026-03-17
**Decision statement:** We will extract export, filtering, and permissions into shared platform services, define a Postgres scaling plan with lead-time-aware triggers, and commit to reliability SLOs -- all sequenced by blast radius so the highest-leverage work ships first, enabling the enterprise push without a firefighting spiral.

---

## 1) Context Snapshot

- **System(s) in scope:** Core B2B analytics SaaS platform -- all product services, the shared Postgres database, and the internal tooling layer consumed by feature teams.
- **Users/customers:** Enterprise and mid-market analytics buyers; internal consumers are ~8-10 feature teams (50 engineers total).
- **Primary pains (1-3):**
  1. **Developer velocity** -- every feature team re-implements export, filtering, and permission checks, creating duplicated effort and inconsistent behavior.
  2. **Database scaling** -- Postgres at 500 GB with increasing query latency; 5x traffic growth expected in 6 months from enterprise push.
  3. **Reliability risk** -- no formal SLOs; enterprise customers will demand con
```

</details>
