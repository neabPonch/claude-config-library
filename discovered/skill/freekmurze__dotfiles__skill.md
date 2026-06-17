---
name: freekmurze__dotfiles__skill
source: https://github.com/freekmurze/dotfiles/blob/ef5ffa09856d06599252e0e2c322f856d7cf355a/config/claude/skills/laravel/SKILL.md
repo: freekmurze/dotfiles
kind: skill
stars: 952
last_pushed: 2026-06-09T12:05:41Z
license: unknown
score: 9
domains: [backend, php, web-framework]
tags: [laravel, mvc, patterns]
curated: 2026-06-15
curated_by: config-scout
---

# freekmurze/dotfiles — skill

**Why it's worth keeping:** Provides concrete code examples for key patterns like Route Model Binding, Form Requests, and Resource Controllers, alongside a specific list of Artisan commands to drive generation.

**Summary:** A comprehensive, pattern-driven guide for Laravel development that covers structure, artisan commands, and coding standards.

**Source credibility:** High; comes from a highly-starred personal dotfiles repository with recent activity.

**Recency:** Current; specifically updated for Laravel 12.

**Source:** [freekmurze/dotfiles/config/claude/skills/laravel/SKILL.md](https://github.com/freekmurze/dotfiles/blob/ef5ffa09856d06599252e0e2c322f856d7cf355a/config/claude/skills/laravel/SKILL.md) · 952★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: laravel
description: Laravel PHP framework conventions and best practices. Use when building Laravel applications, writing controllers, models, migrations, routes, middleware, form requests, policies, jobs, events, or any Laravel-specific code. Triggers include "Laravel", "Eloquent", "Artisan", "php artisan", routing, migrations, or working with Laravel projects.
---

# Laravel 12

Opinionated PHP framework with expressive syntax and well-defined conventions.

## Project Structure

```
app/
├── Http/
│   ├── Controllers/      # Request handlers
│   ├── Middleware/        # HTTP middleware
│   └── Requests/          # Form request validation
├── Models/                # Eloquent models
├── Policies/              # Authorization policies
├── Jobs/                  # Queueable jobs
├── Events/                # Event classes
├── Listeners/             # Event listeners
├── Mail/                  # Mailable classes
└── Providers/             # Service providers
config/                    # Configuration files
database/
├── migrations/            # Database migrations
├── factories/             # Model factories
└── seeders/               # Database seeders
resources/
├── views
```

</details>
