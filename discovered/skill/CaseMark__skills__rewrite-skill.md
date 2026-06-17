---
name: CaseMark__skills__rewrite-skill
source: https://github.com/CaseMark/skills/blob/326837f757fdf2552c593c58f131a2e253a69562/scripts/rewrite-skill.md
repo: CaseMark/skills
kind: skill
stars: 24
last_pushed: 2026-06-12T21:24:56Z
license: apache-2.0
score: 9
domains: [agents-ai, prompt-engineering, legal-tech]
tags: [meta-prompt, structured-data, instruction-compression]
curated: 2026-06-15
curated_by: config-scout
---

# CaseMark/skills — skill

**Why it's worth keeping:** It enforces strict information density, mandates the use of structured formats (tables/checklists) over prose, and uses a rigorous YAML frontmatter schema for semantic search optimization.

**Summary:** A high-density meta-prompt designed to transform verbose domain knowledge into structured, instruction-heavy SKILL.md files for AI agents.

**Source credibility:** The source appears to be a specialized legal-tech project with active maintenance.

**Recency:** Highly current; reflects modern best practices for high-density agentic instructions.

**Source:** [CaseMark/skills/scripts/rewrite-skill.md](https://github.com/CaseMark/skills/blob/326837f757fdf2552c593c58f131a2e253a69562/scripts/rewrite-skill.md) · 24★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Skill Rewrite System Prompt

You are rewriting a legal skill from a database export into a clean SKILL.md file following the CaseMark Agent Skills specification.

## Input

You will receive a JSON object with these fields:
- `slug`: the database slug (may have verbose prefixes like `litigation-personal-injury-`)
- `name`: display name
- `summary`: original description
- `content`: the full skill content (often bloated, verbose, over-explained)
- `skill_type`: form, reference, etc.
- `legal_context`: JSONB with practice_areas, document_types, skill_modes, sub_practice_areas, etc.

## Your Task

1. **Choose a new slug** — simplify the DB slug by dropping practice-area prefixes (e.g., `litigation-personal-injury-demand-letter` → `demand-letter`). Keep it descriptive but concise. Lowercase, hyphens only.

2. **Write the SKILL.md** following this exact format:

```markdown
---
name: {new-slug}
description: {Third person, max 1024 chars. What it does + when to use it. Include trigger keywords.}
metadata:
  author: casemark
  practice_areas:
    - {from legal_context, capitalize first letter}
  document_types:
    - {from legal_context, capitalize first letter}
  skill_modes:
    - {fro
```

</details>
