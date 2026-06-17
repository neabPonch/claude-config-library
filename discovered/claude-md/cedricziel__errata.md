---
name: cedricziel__errata
source: https://github.com/cedricziel/errata/blob/61cd89e4fee1b4f46fcfc23e5d5e11cb071dde22/CLAUDE.md
repo: cedricziel/errata
kind: claude-md
stars: 0
last_pushed: 2026-06-16T06:34:10Z
license: unknown
score: 8
domains: [backend-api, mobile-sdk, php, swift]
tags: [monorepo, architecture, data-flow]
curated: 2026-06-16
curated_by: config-scout
---

# cedricziel/errata — claude-md

**Why it's worth keeping:** The inclusion of data flow sequences and specific test fixture capabilities allows the AI to understand system state changes effectively.

**Summary:** Provides clear command-line workflows and a detailed breakdown of a dual-storage monorepo architecture.

**Source credibility:** Niche project with fresh activity; content is clearly authored for human/AI context rather than generated.

**Recency:** Current; fits modern agentic workflows perfectly.

**Source:** [cedricziel/errata/CLAUDE.md](https://github.com/cedricziel/errata/blob/61cd89e4fee1b4f46fcfc23e5d5e11cb071dde22/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

Errata is an iOS issue monitoring platform (crash reporting, error tracking, performance monitoring). This monorepo contains a Symfony backend and Swift iOS SDK.

## Key Commands

```bash
make install    # Install PHP dependencies (composer install)
make lint       # Run php-cs-fixer --dry-run + PHPStan
make format     # Run php-cs-fixer to fix code style
make test       # Run all PHPUnit tests
make serve      # Start Symfony dev server (requires symfony CLI)
make migrate    # Run database migrations
make db-reset   # Drop, create, and migrate database

# Run a single test or test file
cd apps/server && vendor/bin/phpunit tests/Integration/Api/EventControllerTest.php
cd apps/server && vendor/bin/phpunit --filter testMethodName

# iOS SDK
make sdk-build  # Build Swift package
make sdk-test   # Run Swift tests
```

## Architecture

### Data Flow

1. iOS SDK sends events to `POST /api/v1/events` with `X-Errata-Key` header
2. `EventController` validates and dispatches `ProcessEvent` message to Symfony Messenger
3. `ProcessEventHandler` generates fingerprint,
```

</details>
