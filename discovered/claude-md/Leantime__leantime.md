---
name: Leantime__leantime
source: https://github.com/Leantime/leantime/blob/35ac6abd9478f6a2da295aa55dcaed4196817b90/CLAUDE.md
repo: Leantime/leantime
kind: claude-md
stars: 10022
last_pushed: 2026-06-14T19:12:07Z
license: agpl-3.0
score: 9
domains: [web-app, backend-php, legacy-migration]
tags: [architectural-context, technical-debt-management, developer-onboarding]
curated: 2026-06-15
curated_by: config-scout
---

# Leantime/leantime — claude-md

**Why it's worth keeping:** The 'Active Migrations' section is exceptional; it tells Claude exactly what the target pattern is (HTMX/Blade) vs current reality, preventing useless refactoring suggestions. The structured directory map and specific command groupings make task execution highly reliable.

**Summary:** Provides deep architectural context specifically focused on ongoing migrations to prevent AI from misinterpreting legacy patterns as errors. It serves as a 'state-of-the-union' for the codebase.

**Source credibility:** High-quality open source project with high star count and active recent maintenance.

**Recency:** Very current; reflects modern PHP/Laravel ecosystems and contemporary frontend trends like HTMX.

**Source:** [Leantime/leantime/CLAUDE.md](https://github.com/Leantime/leantime/blob/35ac6abd9478f6a2da295aa55dcaed4196817b90/CLAUDE.md) · 10022★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## About Leantime

Leantime is an open source project management system designed for non-project managers. It combines strategy, planning, and execution in an easy-to-use interface. The application is built with PHP (Laravel), MySQL, and a JS frontend. Current version: 3.6.2.

## Current State & Active Migrations

These are ongoing architectural efforts. None need to be fixed proactively -- they provide context for understanding why the codebase has mixed patterns.

### 1. HTMX Migration (In Progress)
**Goal**: Replace jQuery AJAX and full-page reloads with HTMX partial updates.
**Status**: 8 of 42 domains have dedicated `Hxcontrollers/` with 19 total HxControllers. ~57 Blade templates and ~14 tpl.php files use HTMX attributes.
**Domains with HxControllers**: Tickets, Projects, Timesheets, Widgets, Menu, Notifications, Plugins, Help.
**Pattern**: Main page controllers load minimal data + skeleton; content loads via HTMX partials. New async work should use HTMX, not jQuery AJAX.

### 2. Template Migration (In Progress)
**Goal**: Move from legacy `.tpl.php` to Laravel
```

</details>
