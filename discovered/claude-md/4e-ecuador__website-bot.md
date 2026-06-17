---
name: 4e-ecuador__website-bot
source: https://github.com/4e-ecuador/website-bot/blob/4c2936e728d082738a30bf3fd7109dcde44facb6/CLAUDE.md
repo: 4e-ecuador/website-bot
kind: claude-md
stars: 2
last_pushed: 2026-03-22T02:50:41Z
license: unknown
score: 8
domains: [web-application, backend]
tags: [symfony, php, architecture, workflow]
curated: 2026-06-16
curated_by: config-scout
---

# 4e-ecuador/website-bot — claude-md

**Why it's worth keeping:** Includes specific code quality constraints (cognitive complexity limits) and concrete task workflows like 'Adding New Badges'.

**Summary:** Defines tech stack, development commands, and architectural patterns for a Symfony/Telegram project.

**Source credibility:** Low star count, but the technical depth suggests a professionally managed personal project.

**Recency:** Highly current; uses modern PHP 8.2+ and Symfony 7 standards.

**Source:** [4e-ecuador/website-bot/CLAUDE.md](https://github.com/4e-ecuador/website-bot/blob/4c2936e728d082738a30bf3fd7109dcde44facb6/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

A Symfony 7 web application and Telegram bot for the Ingress game community in Ecuador. Manages agents, badges/medals, events, and challenges.

- **PHP 8.2+** with Symfony 7.x (MicroKernel)
- **PostgreSQL 16** via Docker (docker-compose.yaml)
- **Frontend:** Stimulus JS, Bootstrap 5, Leaflet maps, FullCalendar

## Commands

### Development Setup
```bash
composer install
yarn && yarn dev
docker-compose up -d              # PostgreSQL database
symfony server:start -d
```

### Testing
```bash
make tests                        # Full CI: PHPUnit + PHPStan + Rector
symfony php vendor/bin/phpunit    # Run tests only
symfony php vendor/bin/phpunit --filter=TestName  # Single test
vendor/bin/phpstan analyse        # Static analysis (level 7)
vendor/bin/rector process --dry-run  # Check code modernization
```

### Database
```bash
symfony console doctrine:migrations:migrate
symfony console doctrine:fixtures:load
```

### Translations
```bash
composer translate                # Extract translations (en, es, de)
```

### Update Badge Data
```bash
bin/consol
```

</details>
