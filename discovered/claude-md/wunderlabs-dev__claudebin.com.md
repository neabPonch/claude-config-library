---
name: wunderlabs-dev__claudebin.com
source: https://github.com/wunderlabs-dev/claudebin.com/blob/c04f1d083bfc3f9a536c1e86dbb08d9064e578ee/CLAUDE.md
repo: wunderlabs-dev/claudebin.com
kind: claude-md
stars: 66
last_pushed: 2026-05-27T13:51:03Z
license: mit
score: 9
domains: [web-frontend, typescript, nextjs]
tags: [patterns, frontend, style-guide]
curated: 2026-06-15
curated_by: config-scout
---

# wunderlabs-dev/claudebin.com — claude-md

**Why it's worth keeping:** Uses concrete 'GOOD/BAD' code examples for complex type patterns and styling logic; establishes explicit naming conventions to prevent file structure drift.

**Summary:** Provides strict architectural mapping and high-density coding patterns for a Next.js TypeScript application.

**Source credibility:** Solid; the repository is an active, well-structured open-source tool.

**Recency:** Highly current, referencing modern tools like Turbopack and Oxlint.

**Source:** [wunderlabs-dev/claudebin.com/CLAUDE.md](https://github.com/wunderlabs-dev/claudebin.com/blob/c04f1d083bfc3f9a536c1e86dbb08d9064e578ee/CLAUDE.md) · 66★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Claudebin is a "pastebin for vibes" - a web app for publishing and sharing Claude Code sessions.

## Commands

```bash
# Development
bun dev               # Start web app in dev mode

# Build
bun build             # Build the app

# Code Quality
bun check             # Oxlint and Oxfmt check (runs on pre-commit)
bun format            # Oxfmt format
bun lint              # Oxlint lint
bun type-check        # TypeScript check
```

## Architecture

**Structure:**

- `app/` - Next.js 16 web app (App Router, Turbopack)
- `docs/` - Architecture documentation
- `supabase/` - Database migrations

**App Structure (`app/src/`):**

```
src/
├── app/          # Next.js App Router pages
├── components/   # Reusable UI components
│   └── ui/       # shadcn/ui components
├── sections/     # Page-level section components
├── utils/        # Utilities, constants, helpers
├── copy/         # i18n translations (en-EN.json)
├── i18n/         # i18n config
└── static/       # CSS, fonts
```

**Key Libraries:**

- Web: next-intl, shadcn/ui (Base UI), Tailwind CSS
- Da
```

</details>
