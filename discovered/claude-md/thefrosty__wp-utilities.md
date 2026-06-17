---
name: thefrosty__wp-utilities
source: https://github.com/thefrosty/wp-utilities/blob/1d33158468c9ae40ed496b71eb19b2a24b4f5546/CLAUDE.md
repo: thefrosty/wp-utilities
kind: claude-md
stars: 17
last_pushed: 2026-06-14T00:12:43Z
license: unknown
score: 8
domains: [backend, php]
tags: [architecture-patterns, testing-guidance, wordpress]
curated: 2026-06-15
curated_by: config-scout
---

# thefrosty/wp-utilities — claude-md

**Why it's worth keeping:** Includes concrete code snippets for the fluent interface pattern and mandates a specific test class hierarchy to ensure consistency.

**Summary:** Defines a custom plugin factory architecture and provides specific commands for testing and linting.

**Source credibility:** Active single-developer utility library with very recent updates.

**Recency:** Highly current, utilizing latest PHP 8.4 and PHPUnit standards.

**Source:** [thefrosty/wp-utilities/CLAUDE.md](https://github.com/thefrosty/wp-utilities/blob/1d33158468c9ae40ed496b71eb19b2a24b4f5546/CLAUDE.md) · 17★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Setup

This is a PHP library for WordPress development that provides utilities for building high-quality WordPress plugins. It
requires PHP >= 8.4 and WordPress 6.9 or higher.

## Key Architecture Components

The library follows a plugin factory pattern with a container-based architecture:

1. **Plugin Factory System** - Uses `PluginFactory` to create and manage plugin instances
2. **Hook Registration** - Core `Init` class handles registration and initialization of hook providers
3. **Hook Provider Pattern** - Classes implement `WpHooksInterface` to register WordPress hooks
4. **Container Support** - Integration with PSR-11 containers (Pimple) for dependency injection

## How to Run Tests

Make sure Docker is running with: `docker compose up -d`.

To run the full PHPUnit test suite (with code coverage):

```
composer phpunit
```

To run a specific test:

```
./vendor/bin/phpunit tests/unit/Plugin/PluginTest.php
```

## Common Development Tasks

The library provides a fluent interface for hook registration:

```php
use TheFrosty\WpUtilities\Plugin\Plugi
```

</details>
