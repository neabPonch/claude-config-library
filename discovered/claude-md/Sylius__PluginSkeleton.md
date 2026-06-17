---
name: Sylius__PluginSkeleton
source: https://github.com/Sylius/PluginSkeleton/blob/ad98a823a413df3ea5370ee542f592c03bc1441b/CLAUDE.md
repo: Sylius/PluginSkeleton
kind: claude-md
stars: 85
last_pushed: 2026-02-05T16:00:46Z
license: mit
score: 8
domains: [backend, php, symfony]
tags: [skeleton, docker, testing-framework]
curated: 2026-06-15
curated_by: config-scout
---

# Sylius/PluginSkeleton — claude-md

**Why it's worth keeping:** Uses a dual-path approach (Docker vs. Traditional) to prevent environment execution errors. Includes highly specific test commands including critical JS/non-JS distinctions for Behat.

**Summary:** Provides comprehensive command mappings for both Docker and local environments alongside architectural context. It covers database initialization, testing hierarchies, and code quality tools.

**Source credibility:** High; part of an established, well-maintained e-commerce plugin skeleton.

**Recency:** Current; aligns with modern PHP toolchains and Claude Code's workflow capabilities.

**Source:** [Sylius/PluginSkeleton/CLAUDE.md](https://github.com/Sylius/PluginSkeleton/blob/ad98a823a413df3ea5370ee542f592c03bc1441b/CLAUDE.md) · 85★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

### Docker Environment (Recommended)
```bash
# Initialize Docker environment and install dependencies
make init

# Initialize database and run migrations
make database-init

# Load fixtures (optional)
make load-fixtures

# Start/stop containers
make up
make down

# Access containers
make php-shell
make node-shell
```

### Traditional Development
```bash
# Frontend setup
(cd vendor/sylius/test-application && yarn install)
(cd vendor/sylius/test-application && yarn build)
vendor/bin/console assets:install

# Database setup
vendor/bin/console doctrine:database:create
vendor/bin/console doctrine:migrations:migrate -n
vendor/bin/console sylius:fixtures:load -n

# Start server
symfony server:start -d
```

### Testing
```bash
# PHPUnit tests
vendor/bin/phpunit
make phpunit  # Docker

# Behat tests (non-JS)
vendor/bin/behat --strict --tags="~@javascript&&~@mink:chromedriver"
make behat  # Docker

# Behat tests (JS scenarios)
# Requires Chrome headless and symfony server
APP_ENV=test symfony server:start --port=8080 --daemon
vendor/bin/behat --strict
```

</details>
