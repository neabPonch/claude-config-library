---
name: C00ldudeNoonan__economic-data-project__dbt-skill
source: https://github.com/C00ldudeNoonan/economic-data-project/blob/a3f5223ec4cee9068b417889a04626d64ee44b1c/.claude/skills/dbt-development/dbt_skill.md
repo: C00ldudeNoonan/economic-data-project
kind: skill
stars: 40
last_pushed: 2026-06-12T20:49:17Z
license: mit
score: 9
domains: [data-engineering, sql, analytics]
tags: [dbt, etl, data-modeling]
curated: 2026-06-15
curated_by: config-scout
---

# C00ldudeNoonan/economic-data-project — skill

**Why it's worth keeping:** Includes strict, actionable rules for model organization (staging/intermediate/marts) and exact naming patterns that ensure enterprise-grade data modeling consistency.

**Summary:** Provides highly structured architectural guidelines for dbt projects, covering layering, naming conventions, and testing patterns.

**Source credibility:** The source is a specialized economic data project with recent activity.

**Recency:** Highly current; follows modern industry standards for dbt-core.

**Source:** [C00ldudeNoonan/economic-data-project/.claude/skills/dbt-development/dbt_skill.md](https://github.com/C00ldudeNoonan/economic-data-project/blob/a3f5223ec4cee9068b417889a04626d64ee44b1c/.claude/skills/dbt-development/dbt_skill.md) · 40★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: dbt-development
description: Expert guidance for developing dbt projects including project structure, model patterns, testing, and best practices. Use when working with dbt models, building data transformations, or setting up dbt projects.
---

# dbt Development Expert

## Quick Reference

### When to Use This Skill
- Building or refactoring dbt models
- Setting up dbt project structure
- Writing SQL transformations in dbt
- Implementing tests and documentation
- Optimizing dbt performance
- Following dbt best practices

## Core Principles

### 1. Project Structure
Organize dbt projects in three primary layers moving from source-conformed to business-conformed:

```
models/
├── staging/          # Source-conformed, atomic building blocks
│   ├── source_a/     # One subdirectory per source system
│   └── source_b/
├── intermediate/     # Purpose-built transformations
│   ├── finance/      # Business domain groupings
│   └── marketing/
└── marts/            # Business-conformed, end-user ready
    ├── core/
    ├── finance/
    └── marketing/
```

### 2. Model Naming Conventions

**Staging Models:**
- Format: `stg_[source]__[entity]s.sql`
- Example: `stg_stripe__payments.sq
```

</details>
