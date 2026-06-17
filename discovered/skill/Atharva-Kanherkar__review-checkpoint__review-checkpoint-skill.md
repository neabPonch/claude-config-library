---
name: Atharva-Kanherkar__review-checkpoint__review-checkpoint-skill
source: https://github.com/Atharva-Kanherkar/review-checkpoint/blob/91269d4e3c8f4976390f2241428202fbdfb503c8/review-checkpoint.skill.md
repo: Atharva-Kanherkar/review-checkpoint
kind: skill
stars: 4
last_pushed: 2026-04-13T10:19:32Z
license: mit
score: 8
domains: [software-engineering, testing, devops]
tags: [workflow, contract-driven, quality-assurance, iterative-development]
curated: 2026-06-16
curated_by: config-scout
---

# Atharva-Kanherkar/review-checkpoint — skill

**Why it's worth keeping:** The 'cumulative review' step forces the agent to validate new changes against all previous steps, catching integration bugs early. The use of a branch-specific markdown contract provides a clear source of truth for both the AI and human reviewers.

**Summary:** Enforces a contract-first development workflow that mandates creating a detailed test spec before coding begins. It uses an iterative checkpoint system to prevent architectural drift during multi-step implementations.

**Source credibility:** Solid niche utility with respectable social proof (4 stars) and recent maintenance.

**Recency:** Highly current; aligns perfectly with modern agentic workflows in Claude Code.

**Source:** [Atharva-Kanherkar/review-checkpoint/review-checkpoint.skill.md](https://github.com/Atharva-Kanherkar/review-checkpoint/blob/91269d4e3c8f4976390f2241428202fbdfb503c8/review-checkpoint.skill.md) · 4★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: review-checkpoint
description: >
  Enforces a structured, self-reviewing implementation workflow for coding tasks.
  Use this skill whenever the user asks to implement a feature, fix a bug, build
  something, or work on any coding task that will result in a PR or commit — especially
  multi-step tasks. Also trigger when the user mentions "review checkpoint", "iterative
  review", "testing.md", "reviewcheckpoint", or asks Claude to "review as you go",
  "test before PR", or "write tests first then implement". This skill ensures nothing
  ships without being reviewed against locked expectations. Use it even when the user
  just says "implement this" or "build this feature" on a non-trivial task — the
  discipline of writing expectations first and reviewing iteratively catches bugs
  that post-hoc review misses.
---

# Review Checkpoint — Iterative Implementation with Built-in Review

This skill enforces a disciplined workflow: lock expectations first, implement in
reviewed increments, and only ship when reality matches the contract. Every step
gets reviewed against the previous step and against the original expectations.

## Why This Workflow Exists

Most implementation bug
```

</details>
