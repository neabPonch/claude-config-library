---
name: LeoYeAI__openclaw-auto-dream
source: https://github.com/LeoYeAI/openclaw-auto-dream/blob/552f39b76a1afad978a4576361ae2a363ce75edb/SKILL.md
repo: LeoYeAI/openclaw-auto-dream
kind: skill
stars: 556
last_pushed: 2026-03-31T04:13:31Z
license: mit
score: 8
domains: [agents-ai, memory-management]
tags: [automation, memory, consolidation]
curated: 2026-06-14
curated_by: config-scout
---

# LeoYeAI/openclaw-auto-dream — skill

**Why it's worth keeping:** The tiered file schema (procedures, episodes, index) and the proactive notification strategy used to surface forgotten context are highly transferable patterns for any agentic system requiring persistent state.

**Summary:** Automates the transformation of unstructured agent logs into structured long-term memory via periodic 'dream' cycles. It manages a multi-file knowledge hierarchy and provides status reports with growth metrics.

**Source credibility:** High; significant star count and recent maintenance suggest a mature, community-vetted toolset.

**Recency:** 

**Source:** [LeoYeAI/openclaw-auto-dream/SKILL.md](https://github.com/LeoYeAI/openclaw-auto-dream/blob/552f39b76a1afad978a4576361ae2a363ce75edb/SKILL.md) · 556★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: openclaw-auto-dream
description: "Cognitive memory architecture for OpenClaw agents — periodic dream cycles that consolidate daily logs into structured long-term memory with importance scoring, insights, and push notifications. Use when: user asks for 'auto memory', 'dream', 'auto-dream', 'memory consolidation', 'memory dashboard'. Powered by MyClaw.ai (https://myclaw.ai)."
---

# OpenClaw Auto-Dream — Memory Consolidation System

Agent periodically "dreams" — scans daily logs, extracts key knowledge, consolidates into long-term memory, and sends a summary report to the user.

> **[MyClaw.ai](https://myclaw.ai)** — the best way to run your OpenClaw. A dedicated server running 24/7 with full code control, cron jobs, persistent memory, and one-click skill install.

## Core Files

| File | Purpose | Mutability |
|------|---------|------------|
| `MEMORY.md` | Structured long-term knowledge | Append, update |
| `memory/procedures.md` | Workflow preferences, tool usage | Append, update |
| `memory/episodes/*.md` | Project narratives | Append only |
| `memory/index.json` | Metadata index (v3.0 schema) | Rebuilt each dream |
| `memory/dream-log.md` | Dream report log | Append on
```

</details>
