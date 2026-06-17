---
name: ThomasDev-de__bs-calendar
source: https://github.com/ThomasDev-de/bs-calendar/blob/71e6b08aa509d8e985ce77c94ebde5e81f8b0a4e/CLAUDE.md
repo: ThomasDev-de/bs-calendar
kind: claude-md
stars: 24
last_pushed: 2026-06-13T17:55:00Z
license: mit
score: 8
domains: [web-frontend, jquery]
tags: [architecture, plugin, manual-testing]
curated: 2026-06-15
curated_by: config-scout
---

# ThomasDev-de/bs-calendar — claude-md

**Why it's worth keeping:** It explicitly warns against persisting the transient 'extras' object and details the specific event/callback pattern to prevent logic errors. It also provides clear manual verification instructions in lieu of an automated test suite.

**Summary:** Provides deep technical context for a zero-build jQuery plugin, covering internal state management and method dispatching.

**Source credibility:** A specialized, niche utility with recent maintenance.

**Recency:** Current; highly applicable for navigating zero-build or legacy-style web architectures.

**Source:** [ThomasDev-de/bs-calendar/CLAUDE.md](https://github.com/ThomasDev-de/bs-calendar/blob/71e6b08aa509d8e985ce77c94ebde5e81f8b0a4e/CLAUDE.md) · 24★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this project is

`bs-calendar` is a zero-build jQuery plugin for Bootstrap 5. It ships two browser-ready files in `dist/` — there is no bundler, no npm, and no transpilation step.

## Running the demo

```bash
composer install
php -S localhost:8000 router.php
```

Open `http://localhost:8000/`. The `router.php` serves `demo/index.html` at `/` and resolves static assets from `vendor/` and `dist/`.

## Linting

JSHint is configured in `.jshintrc` (ES11, browser + node globals, jQuery and bootstrap as globals). Run it manually against `dist/bs-calendar.js`.

## No automated test suite

There are no unit or integration tests. Verify changes by running the demo and exercising the relevant paths in the browser.

## Code architecture

### Single-file plugin

All plugin logic lives in `dist/bs-calendar.js`. The file is a single IIFE `(function ($) { ... })(jQuery)` that registers the jQuery plugin `$.fn.bsCalendar` and the global namespace `$.bsCalendar`.

### Global namespace — `$.bsCalendar`

Exposed on the jQuery object after the plugin loads:

- `$.bsCalendar.set
```

</details>
