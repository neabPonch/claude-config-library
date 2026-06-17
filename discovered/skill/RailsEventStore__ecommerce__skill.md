---
name: RailsEventStore__ecommerce__skill
source: https://github.com/RailsEventStore/ecommerce/blob/13adab14ea43351f97bc9ea97133eb4850f8ca20/.claude/skills/new-app/SKILL.md
repo: RailsEventStore/ecommerce
kind: skill
stars: 504
last_pushed: 2026-05-27T09:49:48Z
license: mit
score: 9
domains: [backend-api, web-app]
tags: [rails, event-sourcing, cqrs, scaffolding, monorepo]
curated: 2026-06-15
curated_by: config-scout
---

# RailsEventStore/ecommerce — skill

**Why it's worth keeping:** Includes critical post-generation cleanup (removing nested .git), highly specific test helper overrides for in-memory testing, and automated Makefile orchestration.

**Summary:** Provides a comprehensive blueprint for scaffolding new Rails applications within a specialized CQRS/Event Sourcing monorepo architecture.

**Source credibility:** High; comes from the established RailsEventStore/ecommerce repository with significant community interest.

**Recency:** Current; utilizes modern Ruby/Rails patterns and detailed environmental configurations.

**Source:** [RailsEventStore/ecommerce/.claude/skills/new-app/SKILL.md](https://github.com/RailsEventStore/ecommerce/blob/13adab14ea43351f97bc9ea97133eb4850f8ca20/.claude/skills/new-app/SKILL.md) · 504★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: new-app
description: Scaffold a new Rails app with event sourcing, following project conventions (todomvc as reference)
---

# New App Scaffold

## When to use

Use this skill when asked to create a new Rails application in the `apps/` directory. Each app is a standalone Rails application that uses domain modules from `domains/` and the shared `infra` gem.

## Reference

The `apps/todo_mvc` app is the canonical reference. All patterns below are extracted from it.

## Step-by-step process

### 1. Gather requirements

Before writing any code, clarify:
- The **app name** (snake_case, e.g. `crm`, `inventory_tracker`)
- Which **domain modules** it will use (existing ones from `domains/` or new ones to be created)
- What the app **does** at a high level — what entities, what user actions

### 2. Generate the Rails app

Run from the `apps/` directory. The `rails` alias may not work — use the full rbenv path:

```bash
cd apps && /Users/andrzej/.rbenv/versions/3.4.6/bin/rails new {app_name} --database=postgresql --css=tailwind --skip-test-unit
```

**Important post-generation steps:**
- `rails new` creates a nested `.git` directory inside the new app. **Remove it** so the app is p
```

</details>
