---
name: spatie__laravel-sluggable__laravel-boost-skill
source: https://github.com/spatie/laravel-sluggable/blob/2683bb42df2a03e0a3d83de54477d22f648b9d48/docs/laravel-boost-skill.md
repo: spatie/laravel-sluggable
kind: skill
stars: 1546
last_pushed: 2026-06-02T10:33:20Z
license: mit
score: 8
domains: [backend-api, web-development, ai-agents]
tags: [laravel, slugs, workflow-automation]
curated: 2026-06-15
curated_by: config-scout
---

# spatie/laravel-sluggable — skill

**Why it's worth keeping:** It demonstrates how to teach an agent complex, non-obvious workflows like the 'nullable then unique' migration pattern rather than just basic syntax.

**Summary:** Provides highly opinionated domain knowledge for implementing URL slugs in Laravel, covering migrations, traits, and self-healing logic.

**Source credibility:** Extremely high; Spatie is a premier authority in the Laravel ecosystem with highly maintained packages.

**Recency:** Current; explicitly mentions Claude Code and modern PHP attribute patterns.

**Source:** [spatie/laravel-sluggable/docs/laravel-boost-skill.md](https://github.com/spatie/laravel-sluggable/blob/2683bb42df2a03e0a3d83de54477d22f648b9d48/docs/laravel-boost-skill.md) · 1546★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
title: Laravel Boost skill
weight: 7
---

This package ships a [Laravel Boost](https://github.com/laravel/boost) skill that teaches any Boost-aware AI assistant (Claude Code, Cursor, Copilot CLI, Gemini CLI, and others supported by Boost) how to use `laravel-sluggable` correctly.

## Discovery

When your project has both `spatie/laravel-sluggable` and `laravel/boost` installed, Boost's `SkillComposer` automatically discovers the skill at `vendor/spatie/laravel-sluggable/resources/boost/skills/sluggable-development/`. No extra configuration is required.

Running Boost's install command writes the skill into your configured agent's skills directory (for example, `.claude/skills/sluggable-development/` for Claude Code or `.agents/skills/sluggable-development/` for Gemini CLI).

## What the skill covers

The skill activates when a query mentions slugs, permalinks, the `HasSlug` trait, the `HasTranslatableSlug` trait, the `#[Sluggable]` attribute, `SlugOptions`, `findBySlug`, self-healing URLs, or stale slug redirects. It guides the assistant through:

- Choosing between the `#[Sluggable]` attribute and the `HasSlug` trait for a given model.
- Generating the migration for a slug col
```

</details>
