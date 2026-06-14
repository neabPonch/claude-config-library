---
name: DataIntellectTech__TorQ__claude-skill
source: https://github.com/DataIntellectTech/TorQ/blob/b03e47530f664377a5021c498e80b7511a112a9c/docs/claude-skill.md
repo: DataIntellectTech/TorQ
kind: skill
stars: 308
last_pushed: 2026-06-11T15:39:51Z
license: mit
score: 9
domains: [fintech, data-engineering, backend]
tags: [kdb+, q-language, framework-specialization]
curated: 2026-06-14
curated_by: config-scout
---

# DataIntellectTech/TorQ — skill

**Why it's worth keeping:** Uses a modular multi-file strategy (core vs. on-demand) to prevent context bloat; includes professional deployment strategies for distributing skills via submodules or global paths.

**Summary:** Provides domain-specific architectural patterns and lifecycle rules for the TorQ kdb+ production framework to ensure LLM code adheres to proprietary conventions.

**Source credibility:** High; developed by the DataIntellectTech team for their production-grade framework.

**Recency:** Current; aligns with modern Claude Code skill auto-discovery and structure.

**Source:** [DataIntellectTech/TorQ/docs/claude-skill.md](https://github.com/DataIntellectTech/TorQ/blob/b03e47530f664377a5021c498e80b7511a112a9c/docs/claude-skill.md) · 308★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Skill for TorQ

A [Claude Code skill](https://docs.claude.com/en/docs/claude-code/skills) ships with this repo under [.claude/skills/torq-developer/](../.claude/skills/torq-developer/). It teaches Claude the TorQ conventions it wouldn't otherwise know — the guard pattern for config, `.servers.*` for connections, `.timer.repeat` for scheduling, `.api.add` for public functions, the EOD lifecycle, and the two-stage workflow for adding a new process.

With the skill loaded, Claude produces code that fits a TorQ codebase instead of plausible-looking q that ignores the framework.

## What's in the skill

- `SKILL.md` — the core rules (namespace, config, logging, handlers, timers, schemas, subscriptions, connections, gateway patterns, q-language pitfalls, EOD). Always loaded.
- `torq-internals.md` — startup order, EOD sequence, gateway request lifecycle, discovery protocol.
- `torq-patterns.md` — namespace table, IPC and subscription patterns, caching, async helpers, error-trapping idioms.
- `torq-process-templates.md` — `process.csv` columns, `setenv.sh`, `torq.sh` commands, deployment checklist, and templates for minimal process, feedhandler, RDB, WDB, gateway.
- `q-language-re
```

</details>
