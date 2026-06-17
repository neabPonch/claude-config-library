---
name: open-telemetry__opentelemetry-php
source: https://github.com/open-telemetry/opentelemetry-php/blob/2f1c57fda6b2b6172e42996fe4256915a08120b7/CLAUDE.md
repo: open-telemetry/opentelemetry-php
kind: claude-md
stars: 896
last_pushed: 2026-06-13T04:28:46Z
license: apache-2.0
score: 9
domains: [backend, observability, php]
tags: [monorepo, architectural-patterns, testing-lifecycle]
curated: 2026-06-15
curated_by: config-scout
---

# open-telemetry/opentelemetry-php — claude-md

**Why it's worth keeping:** Uses actionable command templates for specific test runs and establishes strict 'Definition of Done' criteria via CI requirements. The architecture section uses a table to clarify monorepo package responsibilities, which prevents dependency errors.

**Summary:** Provides a comprehensive operational manual covering setup, command-line workflows, and detailed architectural hierarchies. It bridges the gap between low-level commands and high-level design patterns.

**Source credibility:** Very high; OpenTelemetry is an industry-standard project with massive adoption and active maintenance.

**Recency:** Extremely relevant for modern tool-use workflows involving Docker, Make, and static analysis.

**Source:** [open-telemetry/opentelemetry-php/CLAUDE.md](https://github.com/open-telemetry/opentelemetry-php/blob/2f1c57fda6b2b6172e42996fe4256915a08120b7/CLAUDE.md) · 896★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Setup

This project uses the "3 Musketeers" pattern: Docker + Make + Compose. Most commands run inside Docker containers.

```bash
cp .env.dist .env   # Required before first use
make install        # Install dependencies
```

Set `PHP_VERSION` (8.1, 8.2, 8.3) to test against specific PHP versions: `PHP_VERSION=8.1 make all`

## Common Commands

```bash
make test           # Unit + integration tests
make test-unit      # Unit tests only
make test-integration # Integration tests only
make style          # Run php-cs-fixer (auto-fix)
make rector-write   # Apply rector refactoring
make deptrac        # Check architectural layer dependencies
make phan           # Phan static analysis
make psalm          # Psalm static analysis
make phpstan        # PHPStan static analysis
make all            # Full CI suite (run before submitting PRs)
make all-lowest     # Same but with lowest dependency versions
```

### Running a single test

```bash
# Run a specific test file
vendor/bin/phpunit tests/Unit/SDK/Trace/SpanTest.php

# Run with a filter
vendor/bin/phpunit --
```

</details>
