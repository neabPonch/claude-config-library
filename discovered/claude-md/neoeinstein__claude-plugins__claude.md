---
name: neoeinstein__claude-plugins__claude
source: https://github.com/neoeinstein/claude-plugins/blob/74587d9ac1f3c6f403783f7a835bab74924e7cb2/plugins/htmx-alpine/CLAUDE.md
repo: neoeinstein/claude-plugins
kind: claude-md
stars: 3
last_pushed: 2026-04-20T16:23:16Z
license: unknown
score: 9
domains: [ai-agent-guidance, web-frontend]
tags: [meta-template, structured-instructions, skill-definition]
curated: 2026-06-15
curated_by: config-scout
---

# neoeinstein/claude-plugins — claude-md

**Why it's worth keeping:** Uses high-signal concepts like Contracts, Invariants, and STOP sections to provide the AI with absolute guardrails against anti-patterns.

**Summary:** A sophisticated blueprint for defining AI 'skills' through formal technical constraints rather than loose documentation.

**Source credibility:** Low star count but demonstrates a highly advanced understanding of agentic prompting structures.

**Recency:** Extremely current/future-dated template designed for modern agentic workflows.

**Source:** [neoeinstein/claude-plugins/plugins/htmx-alpine/CLAUDE.md](https://github.com/neoeinstein/claude-plugins/blob/74587d9ac1f3c6f403783f7a835bab74924e7cb2/plugins/htmx-alpine/CLAUDE.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# htmx-alpine Plugin

Last verified: 2026-02-25

## Purpose

Patterns for building server-driven web applications with HTMX and Alpine.js. Language-agnostic guidance focused on the interaction model, with framework-specific reference docs for common stacks.

## Contracts

- **Exposes**: `htmx-alpine:htmx-alpine` skill with 6 reference docs + 1 framework variant
- **Guarantees**: Skill is standalone, no hooks. Reference docs are lazy-loaded via SKILL.md lookup tables. Core patterns are framework-agnostic.
- **Expects**: User working with HTMX and/or Alpine.js in any server-side framework

## Key Decisions

- **Server is source of truth**: Core principle emphasized throughout. Alpine state is UI-only.
- **Accessibility not optional**: Dedicated reference doc with STOP section. Focus management, ARIA live regions, keyboard navigation.
- **Framework variants as reference docs**: rust-axum.md in frameworks/ subdirectory. Additional variants (Django, Go) can be added incrementally.
- **Cross-plugin soft pointer**: rust-axum.md references askama plugin for template patterns without hard dependency.

## Key Files

- `skills/htmx-alpine/SKILL.md` — Main skill with lookup tables and anti-rat
```

</details>
