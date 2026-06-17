---
name: ChantalSchot__pokopia-tracker__prompt-claude
source: https://github.com/ChantalSchot/pokopia-tracker/blob/cb597e6451c7fe79d5ed58ed70b3b21f77c19bec/prompts/prompt-claude.md
repo: ChantalSchot/pokopia-tracker
kind: claude-md
stars: 0
last_pushed: 2026-04-15T14:01:54Z
license: unknown
score: 9
domains: [full-stack, software-architecture]
tags: [two-phase-flow, structured-spec, high-rigor]
curated: 2026-06-16
curated_by: config-scout
---

# ChantalSchot/pokopia-tracker — claude-md

**Why it's worth keeping:** The two-phase execution model (Phase 1: Analysis/Confirmation -> Phase 2: Implementation) is a premier technique for complex builds, paired with extremely specific data and port constraints.

**Summary:** A high-rigor specification that enforces a mandatory 'Analysis-before-Code' workflow to prevent architectural drift and hallucinations.

**Source credibility:** Individual project repo with no social proof; quality is inferred from technical depth and density.

**Recency:** Very recent (2 months ago).

**Source:** [ChantalSchot/pokopia-tracker/prompts/prompt-claude.md](https://github.com/ChantalSchot/pokopia-tracker/blob/cb597e6451c7fe79d5ed58ed70b3b21f77c19bec/prompts/prompt-claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Sonnet Prompt — Build `pokopia-tracker`

You are a senior full-stack engineer, software architect, product-minded UX engineer, accessibility specialist, DevOps engineer, QA engineer, and technical writer.

Your job is to generate a **fully working, production-quality monorepo** for a web application named **`pokopia-tracker`**.

The output must include **everything needed to clone, configure, run, test, document, and extend the application**. Do **not** give a partial scaffold, pseudo-code, TODO-only structure, or high-level outline. Generate concrete code, concrete files, and concrete documentation.

The stack and requirements below are mandatory unless explicitly challenged during Phase 1 and then confirmed by the user.

---

## Critical working mode: 2-phase flow

You must work in **two distinct phases**.

### Phase 1 — analysis, assumptions, contradictions, decisions

Before generating any code, you must:

1. Read all requirements carefully.
2. Identify:
- assumptions you are making;
- contradictions or ambiguous requirements;
- missing decisions that affect architecture or implementation;
- data-model questions;
- API/security questions;
- UX questions;
- import/data-
```

</details>
