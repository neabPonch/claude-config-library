---
name: SumonMSelim__agentguard__skill
source: https://github.com/SumonMSelim/agentguard/blob/8e26f9aee9e0b2037e0da5193751e5f3aa505633/skills/laravel/SKILL.md
repo: SumonMSelim/agentguard
kind: skill
stars: 47
last_pushed: 2026-06-01T16:38:49Z
license: mit
score: 9
domains: [backend, php, web-framework, architecture]
tags: [laravel, php, best-practices, backend]
curated: 2026-06-15
curated_by: config-scout
---

# SumonMSelim/agentguard — skill

**Why it's worth keeping:** Provides specific technical constraints like using PHP Attributes for jobs/models, enforcing 'strict mode' to prevent N+1, and prescribing exact testing toolsets. The inclusion of new L13 features makes it a cutting-edge reference for AI agents.

**Summary:** Highly opinionated and exhaustive best-practices guide for modern Laravel development (v13+). It covers the entire lifecycle from architecture to production monitoring.

**Source credibility:** The depth of Laravel-specific nuance (e.g., Reverb, Cache::touch) suggests a highly skilled author despite the modest star count.

**Recency:** Extremely current; explicitly targets Laravel 13 and modern PHP attribute usage.

**Source:** [SumonMSelim/agentguard/skills/laravel/SKILL.md](https://github.com/SumonMSelim/agentguard/blob/8e26f9aee9e0b2037e0da5193751e5f3aa505633/skills/laravel/SKILL.md) · 47★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: laravel
tags: []
description: Laravel 13 best practices: architecture, Eloquent, security, queues, testing, tooling. PHP 8.3+. Use when writing or reviewing Laravel applications.
license: MIT
---

# Laravel

## Architecture
- Thin controllers: validate input, call service or action, return response. No business logic in controllers
- Form Requests for validation and authorisation. Never validate in controller body
- Service classes or Actions for domain logic. One responsibility each
- Repositories only when swapping data sources is a real requirement
- No logic in routes or middleware beyond stated purpose
- Strict mode in `AppServiceProvider`: `Model::shouldBeStrict()` in non-production, `Model::preventLazyLoading()` in all envs

## PHP Attributes (Laravel 13+)
- PHP Attributes are optional but preferred for co-locating config with classes
- Models: `#[Fillable]`, `#[Guarded]`, `#[Hidden]` replace `$fillable`, `$guarded`, `$hidden` properties
- Controllers: `#[Middleware]`, `#[Authorize]` replace `$this->middleware()` in constructor
- Jobs: `#[Tries]`, `#[Backoff]`, `#[Timeout]`, `#[FailOnTimeout]` replace class properties
- Adopt Attributes on new code. No need to migr
```

</details>
