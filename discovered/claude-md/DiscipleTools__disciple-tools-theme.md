---
name: DiscipleTools__disciple-tools-theme
source: https://github.com/DiscipleTools/disciple-tools-theme/blob/819fe08932215630144237bb117cd0e4beade917/CLAUDE.md
repo: DiscipleTools/disciple-tools-theme
kind: claude-md
stars: 46
last_pushed: 2026-06-11T10:45:23Z
license: gpl-2.0
score: 9
domains: [wordpress, backend-api, php, web-frontend]
tags: [architecture-mapping, module-system, development-workflows]
curated: 2026-06-15
curated_by: config-scout
---

# DiscipleTools/disciple-tools-theme — claude-md

**Why it's worth keeping:** Excellent use of 'Key Patterns' to explain how modules interact via filters and specific API namespaces; includes practical developer warnings like the lodash/underscore conflict.

**Summary:** Provides a deep architectural mental model of a modular custom WordPress application rather than just a list of files.

**Source credibility:** Active project with recent maintenance and specialized domain context.

**Recency:** Very current, utilizing modern toolchains like Vite and PHP 8.1+.

**Source:** [DiscipleTools/disciple-tools-theme/CLAUDE.md](https://github.com/DiscipleTools/disciple-tools-theme/blob/819fe08932215630144237bb117cd0e4beade917/CLAUDE.md) · 46★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Disciple.Tools is a WordPress theme that functions as a CRM for Christian ministries managing discipleship and church growth. It's not a typical theme—it's a full application built on WordPress.

## Common Commands

### Build & Development
```bash
npm install          # Install dependencies and run build
npm run dev          # Start Vite dev server with HMR (styles only)
npm run build        # Build CSS/JS for production (Vite)
```

### Linting
```bash
npm run lint                    # Run ESLint
npm run prettier                # Format JS files with Prettier
composer install                # Install PHP dependencies (PHPCS, PHPUnit, etc.; requires PHP >= 8.1)
./tests/test_phpcs.sh           # Run PHP CodeSniffer
./tests/test_phpcs.sh file.php  # Run PHPCS on specific files
./vendor/bin/phpcbf             # Auto-fix PHPCS errors
./tests/test_eslint.sh          # Run ESLint + Prettier check
```

### PHPUnit (after WordPress test lib install)
```bash
./tests/install-wp-tests.sh <db-name> <db-user> <db-pass> [db-host]
composer install
composer run t
```

</details>
