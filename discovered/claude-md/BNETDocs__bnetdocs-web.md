---
name: BNETDocs__bnetdocs-web
source: https://github.com/BNETDocs/bnetdocs-web/blob/e51f32dd34a2da5178ee5f64e3f0e422491a2eab/CLAUDE.md
repo: BNETDocs/bnetdocs-web
kind: claude-md
stars: 35
last_pushed: 2026-06-05T09:13:40Z
license: agpl-3.0
score: 9
domains: [backend-api, web-application]
tags: [php, mvc-architecture, request-flow, custom-framework]
curated: 2026-06-14
curated_by: config-scout
---

# BNETDocs/bnetdocs-web — claude-md

**Why it's worth keeping:** The ASCII request flow diagram and exact method/return type definitions prevent the AI from guessing how components interact. It also includes practical linting commands that ensure code quality standards are met during generation.

**Summary:** This file provides a highly detailed technical map of a custom MVC framework including request lifecycle and specific method signatures.

**Source credibility:** Active repository with recent updates and a specialized niche community (35 stars).

**Recency:** Very current; utilizes modern PHP 8.3+ context.

**Source:** [BNETDocs/bnetdocs-web/CLAUDE.md](https://github.com/BNETDocs/bnetdocs-web/blob/e51f32dd34a2da5178ee5f64e3f0e422491a2eab/CLAUDE.md) · 35★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

BNETDocs: Phoenix is a PHP 8.3+ web application for documenting Blizzard Entertainment's Battle.net and in-game protocols. Production site: https://bnetdocs.org

## Commands

### Dependencies
```bash
composer install                    # Install all dependencies
composer update -o --no-dev         # Production update with optimization
```

### Linting
```bash
# Lint a single PHP file
php -e -l -f src/path/to/file.php

# Lint all PHP/PHTML files (mirrors CI)
find src/ -name "*.php" -o -name "*.phtml" | xargs -I{} php -e -l -f {}
```

### Testing
```bash
lib/bin/phpunit                     # Run all tests
```

### Docker (local development)
```bash
docker compose up -d                # Start nginx, PHP-FPM, MariaDB
docker compose down                 # Stop containers
```

## Architecture

### Request Flow

```
HTTP Request → Nginx (FastCGI) → PHP-FPM → src/main.php
  → Router::invoke()
  → Pattern-matched Controller::invoke($args)    # sets $model data
  → Content-negotiated View::invoke($model)      # renders output
  → Response with headers and
```

</details>
