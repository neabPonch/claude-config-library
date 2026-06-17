---
name: afragen__git-updater
source: https://github.com/afragen/git-updater/blob/d6cb80e09164c699d97f46a67979f0a089a74f34/CLAUDE.md
repo: afragen/git-updater
kind: claude-md
stars: 3318
last_pushed: 2026-06-13T18:02:12Z
license: gpl-3.0
score: 9
domains: [php, wordpress, devops, testing]
tags: [wordpress, phpunit, phpstan, docker]
curated: 2026-06-16
curated_by: config-scout
---

# afragen/git-updater — claude-md

**Why it's worth keeping:** Includes specific environmental nuances like test polyfills and provides explicit, transferable instructions for PHPStan type-hinting standards to ensure code quality during AI refactors.

**Summary:** Provides strict confidence guardrails and highly detailed command maps for a complex WordPress Docker environment.

**Source credibility:** High; the repository is well-established with significant stars and active maintenance.

**Recency:** Current; perfectly tailored for modern agentic tool use and modern PHP/JS ecosystems.

**Source:** [afragen/git-updater/CLAUDE.md](https://github.com/afragen/git-updater/blob/d6cb80e09164c699d97f46a67979f0a089a74f34/CLAUDE.md) · 3318★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## General Instructions

Do not make any changes until you have 95% confidence in what you need to build. Ask me follow-up questions until you reach that confidence.

## Commands

```sh
# Install PHP dependencies
composer install

# Install JS dependencies (required for wp-env)
npm install

# Lint (PHPCS)
composer lint

# Auto-fix linting issues (PHPCBF)
composer format

# Static analysis
composer phpstan

# Regenerate PHPStan baseline (after intentional changes that add new errors)
composer phpstan-baseline

# Run PHPUnit tests via wp-env (single site)
composer test          # delegates to: npm test
npm test

# Run PHPUnit tests via wp-env (multisite)
composer test-ms       # delegates to: npm run test:multisite
npm run test:multisite

# Run PHPUnit tests with code coverage (requires Xdebug — installed automatically on wp-env start)
npm run test:coverage

# Start/stop wp-env Docker environment
# Note: afterStart lifecycle script installs Xdebug into the tests-cli container
npm run wp-env start
npm run wp-env stop

# Run a single test class or method
# Use npm test w
```

</details>
