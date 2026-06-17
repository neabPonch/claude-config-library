---
name: CherryHQ__cherry-studio
source: https://github.com/CherryHQ/cherry-studio/blob/1ad784437bdfb3e410cb14e71419e1c3d9979ec0/CLAUDE.md
repo: CherryHQ/cherry-studio
kind: claude-md
stars: 47340
last_pushed: 2026-06-15T04:46:37Z
license: agpl-3.0
score: 9
domains: [web-app, desktop-app, ai-productivity]
tags: [surgical-coding, mental-models, monorepo, operational-rules]
curated: 2026-06-15
curated_by: config-scout
---

# CherryHQ/cherry-studio — claude-md

**Why it's worth keeping:** The 'Surgical Changes' principle prevents LLM drift/bloat, while the task-to-goal conversion pattern ensures verifiable outcomes. It also effectively uses local README links to deepen context.

**Summary:** Establishes rigorous mental models for surgical coding and provides strict operational constraints for a complex monorepo.

**Source credibility:** Highly credible; high star count and very active maintenance.

**Recency:** Extremely current based on repository activity.

**Source:** [CherryHQ/cherry-studio/CLAUDE.md](https://github.com/CherryHQ/cherry-studio/blob/1ad784437bdfb3e410cb14e71419e1c3d9979ec0/CLAUDE.md) · 47340★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
## Guiding Principles (MUST FOLLOW)

### Mindset

How to approach any coding task in this repo.

#### Think Before Coding

- State assumptions explicitly. If uncertain, ask before implementing.
- When multiple interpretations exist, surface them — do not pick silently.
- If a simpler approach exists, say so. Push back when warranted.
- If something is unclear, stop. Name what is confusing. Ask.

#### Simplicity First

- Write the minimum code that solves the problem. Nothing speculative.
- No features beyond what was asked.
- No abstractions for single-use code.
- No "flexibility" or "configurability" that was not requested.
- No error handling for impossible scenarios.
- If you wrote 200 lines and it could be 50, rewrite it.

#### Surgical Changes

- Touch only what the task requires. Do not "improve" adjacent code, comments, or formatting.
- Do not refactor things that are not broken.
- Match existing style even if you would do it differently.
- If you notice unrelated dead code, mention it — do not delete it.
- Remove imports / variables / functions that **your** changes orphaned. Leave pre-existing dead code alone unless asked.
- Every changed line must trace directly to the us
```

</details>
