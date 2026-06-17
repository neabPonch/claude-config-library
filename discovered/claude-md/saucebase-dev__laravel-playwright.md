---
name: saucebase-dev__laravel-playwright
source: https://github.com/saucebase-dev/laravel-playwright/blob/471614ecad25e5c0e960bd5bb7aff9f37cba2cf6/CLAUDE.md
repo: saucebase-dev/laravel-playwright
kind: claude-md
stars: 2
last_pushed: 2026-04-30T19:31:12Z
license: mit
score: 8
domains: [backend, testing, php, typescript]
tags: [cross-language, e2e-testing, architectural-context]
curated: 2026-06-15
curated_by: config-scout
---

# saucebase-dev/laravel-playwright — claude-md

**Why it's worth keeping:** The 'How it works' section explains data flow and side effects, while the explicit PHPStan type requirements prevent common AI-generated static analysis errors.

**Summary:** Provides a deep architectural map of a dual-language (PHP/TypeScript) system, explaining how state is bridged between the two environments. It includes specific instructions for maintaining high static analysis standards.

**Source credibility:** A specialized developer tool; though low in stars, the documentation is highly structured and technical.

**Recency:** Very current (2 months ago), aligning well with modern Claude Code workflows.

**Source:** [saucebase-dev/laravel-playwright/CLAUDE.md](https://github.com/saucebase-dev/laravel-playwright/blob/471614ecad25e5c0e960bd5bb7aff9f37cba2cf6/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Git

- Commit messages must be a single line — no body, no bullet points
- No `Co-Authored-By` or AI attribution lines in commits — the commit author is the human user, even if an AI assistant contributed to the code
- Commits should use conventional commit style, e.g. `feat: add time travel endpoint` or `fix: handle missing sqlite_sequence table`

## Commands

```bash
# PHP tests
./vendor/bin/phpunit                          # all tests
./vendor/bin/phpunit --filter=SecurityTest    # single test class
./vendor/bin/phpunit --filter=testRunsAQuery  # single test method

# Static analysis (max level, covers src/ and tests/)
./vendor/bin/phpstan analyse --memory-limit=512M

# JS/TS build (outputs to dist/)
npm run build   # tsc type-check + vite build
```

## Architecture

This is a dual-language package: a **PHP Laravel package** (`src/`) paired with a **TypeScript Playwright client** (`src/playwright/src/`).

### How it works

The PHP side registers HTTP routes (under a configurable prefix, default `playwright/`) that are only active in configured environments (`lo
```

</details>
