---
name: zscole__model-hierarchy-skill
source: https://github.com/zscole/model-hierarchy-skill/blob/9095f8303847a60de9f564659e561f3f6fd0cdc4/SKILL.md
repo: zscole/model-hierarchy-skill
kind: skill
stars: 339
last_pushed: 2026-02-16T16:55:41Z
license: mit
score: 9
domains: [agents-ai, cost-optimization]
tags: [model-routing, orchestration]
curated: 2026-06-14
curated_by: config-scout
---

# zscole/model-hierarchy-skill — skill

**Why it's worth keeping:** The taxonomy of task classification (Routine/Moderate/Complex) and the specific behavioral rules for proposing model shifts are excellent meta-skills for any autonomous agent.

**Summary:** An orchestration framework that routes tasks through tiered model levels based on complexity, vision needs, and historical success.

**Source credibility:** High social proof with 339 stars and a highly structured, professional documentation style.

**Recency:** Uses future-dated pricing (Feb 2026), making it a speculative/forward-looking template rather than an up-to-the-minute price sheet.

**Source:** [zscole/model-hierarchy-skill/SKILL.md](https://github.com/zscole/model-hierarchy-skill/blob/9095f8303847a60de9f564659e561f3f6fd0cdc4/SKILL.md) · 339★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: model-hierarchy
description: >
  Cost-optimize AI agent operations by routing tasks to appropriate models based on complexity.
  Use this skill when: (1) deciding which model to use for a task, (2) spawning sub-agents,
  (3) considering cost efficiency, (4) the current model feels like overkill for the task.
  Triggers: "model routing", "cost optimization", "which model", "too expensive", "spawn agent".

---

# Model Hierarchy

Route tasks to the cheapest model that can handle them. Most agent work is routine.

## Core Principle

**80% of agent tasks are janitorial.** File reads, status checks, formatting, simple Q&A. These don't need expensive models. Reserve premium models for problems that actually require deep reasoning.

## Model Tiers

### Tier 1: Cheap ($0.10-0.50/M tokens)

| Model | Input | Output | Best For |
|-------|-------|--------|----------|
| DeepSeek V3 | $0.14 | $0.28 | General routine work |
| GPT-4o-mini | $0.15 | $0.60 | Quick responses |
| Claude Haiku | $0.25 | $1.25 | Fast tool use |
| Gemini Flash | $0.075 | $0.30 | High volume |
| GLM 5 (Zhipu) | (OpenRouter Z.AI) | (OpenRouter Z.AI) | Routine + moderate text; 200K context; **text-only** — do not
```

</details>
