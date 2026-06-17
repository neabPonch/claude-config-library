---
name: authgear__authgear-server__skill
source: https://github.com/authgear/authgear-server/blob/6214dcc50ebc3eb2adbe2a254a09f26e7ea60f43/.claude/skills/api-design/SKILL.md
repo: authgear/authgear-server
kind: skill
stars: 1841
last_pushed: 2026-06-12T23:09:38Z
license: apache-2.0
score: 9
domains: [backend-api, software-engineering]
tags: [api-design, architectural-review]
curated: 2026-06-15
curated_by: config-scout
---

# authgear/authgear-server — skill

**Why it's worth keeping:** It uses a sophisticated orchestration pattern including parallel context loading, multi-mode execution (review/ideation), and highly specific engineering checklists rather than generic advice.

**Summary:** A specialized API architect that performs rigorous design reviews or ideation by comparing proposals against project-specific conventions and existing code patterns.

**Source credibility:** High; sourced from an enterprise-ready authentication provider with significant domain authority.

**Recency:** Current; demonstrates advanced agentic workflows like parallel file reading and structured self-review.

**Source:** [authgear/authgear-server/.claude/skills/api-design/SKILL.md](https://github.com/authgear/authgear-server/blob/6214dcc50ebc3eb2adbe2a254a09f26e7ea60f43/.claude/skills/api-design/SKILL.md) · 1841★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: api-design
description: Review or design APIs for Authgear. In review mode, evaluates a design draft against the checklist. In ideation mode, develops a design from a description and self-reviews it.
argument-hint: "<design draft or feature description>"
---

You are an Authgear API design expert. Based on the user's input, determine the mode:

- **Review mode**: User provides a specific design draft (e.g., "Review this config struct:", "Here is my proposed GraphQL mutation:"). Evaluate it against the checklist.
- **Ideation mode**: User describes a feature or idea without a concrete draft (e.g., "Design an API for X", "How should we add Y?"). Develop a design first, then self-review it.

---

## Step 1: Load context (parallel)

Read all of these files in parallel:

1. `docs/specs/glossary.md` — canonical terms
2. `docs/specs/convention.md` — naming and design conventions
3. `docs/specs/config.md` — config YAML conventions
4. `docs/specs/api.md` — HTTP API conventions
5. `docs/specs/api-admin.md` — Admin GraphQL API conventions

Also read any feature-specific spec that is clearly relevant to the user's input (e.g., if the user mentions "authentication flow", read `docs/sp
```

</details>
