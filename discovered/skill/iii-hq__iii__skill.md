---
name: iii-hq__iii__skill
source: https://github.com/iii-hq/iii/blob/29fb4c922578a85077a2dce3f6af5cf09fbc6db7/engine/src/workers/cron/skills/SKILL.md
repo: iii-hq/iii
kind: skill
stars: 18116
last_pushed: 2026-06-14T21:04:28Z
license: unknown
score: 8
domains: [backend, distributed-systems, scheduling]
tags: [cron, redis, task-scheduler, typescript]
curated: 2026-06-15
curated_by: config-scout
---

# iii-hq/iii — skill

**Why it's worth keeping:** The 'Boundaries' section provides high-value guardrails that prevent common errors like incorrect cron field counts or improper adapter usage.

**Summary:** A technical specification for a cron-based task scheduler that handles distributed execution across a fleet using Redis locks.

**Source credibility:** High; the source repository has 18k stars, indicating a widely-used and stable system.

**Recency:** Current; it utilizes modern async patterns (Tokio) and distributed systems logic relevant to contemporary environments.

**Source:** [iii-hq/iii/engine/src/workers/cron/skills/SKILL.md](https://github.com/iii-hq/iii/blob/29fb4c922578a85077a2dce3f6af5cf09fbc6db7/engine/src/workers/cron/skills/SKILL.md) · 18116★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: iii-cron
description: >-
  Schedule any registered function on a 6- or 7-field cron expression, with
  once-only execution across a fleet when backed by the redis adapter. Its whole
  surface is the `cron` trigger type.
---

# iii-cron

The `iii-cron` worker schedules a registered function to run on a recurring cron expression. It exposes no callable functions — its entire surface is one trigger type, `cron`, bound via `iii.registerTrigger({ type: 'cron', function_id, config })`. On every firing the engine builds an event payload, optionally evaluates a condition function, acquires a distributed lock through the configured adapter, and invokes the target function. Each firing reports `scheduled_time` vs. `actual_time` so drift and reentrancy are observable from inside the handler.

The schedule grammar is the seven-field cron dialect — `second minute hour day-of-month month day-of-week [year]` — where the year is optional and defaults to `*`. Both six- and seven-field forms work; the leading field is always seconds, so `0 */5 * * * *` fires every 5 minutes at second 0, not every 5 seconds.

Two adapters govern once-only execution: `kv` (default) takes a process-local lock
```

</details>
