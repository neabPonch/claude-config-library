---
name: archtechx__tenancy
source: https://github.com/archtechx/tenancy/blob/652bc987cedb19d345bcb1a948ad02a6ce40e238/CLAUDE.md
repo: archtechx/tenancy
kind: claude-md
stars: 4355
last_pushed: 2026-06-13T07:26:44Z
license: mit
score: 9
domains: [backend, php, laravel]
tags: [architecture-patterns, environment-setup, gotchas]
curated: 2026-06-14
curated_by: config-scout
---

# archtechx/tenancy — claude-md

**Why it's worth keeping:** It includes proactive warnings about non-obvious architectural pitfalls (Early Identification) and provides actual code patterns for runtime state management.

**Summary:** Provides deep architectural context, specific command shortcuts, and crucial 'gotchas' regarding Laravel lifecycle timing.

**Source credibility:** Highly credible: a widely used industry-standard library with high star count and active maintenance.

**Recency:** Current; provides highly relevant technical guidance for modern LLM coding agents.

**Source:** [archtechx/tenancy/CLAUDE.md](https://github.com/archtechx/tenancy/blob/652bc987cedb19d345bcb1a948ad02a6ce40e238/CLAUDE.md) · 4355★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

### Testing
- `composer test` - Run tests without coverage using Docker
- `./test tests/TestFile.php` - Run an entire test file
- `./t 'test name'` - Run a specific test
- You can append `-v` to get a full stack trace if a test fails due to an exception

### Code Quality
- `composer phpstan` - Run PHPStan static analysis (level 8)
- `composer cs` - Fix code style using PHP CS Fixer

### Docker Development
- `composer docker-up` - Start Docker environment
- `composer docker-down` - Stop Docker environment
- `composer docker-restart` - Restart Docker environment

## Architecture Overview

**Tenancy for Laravel** is a multi-tenancy package that automatically handles tenant isolation without requiring changes to application code.

### Core Components

**Central Classes:**
- `Tenancy` - Main orchestrator class managing tenant context and lifecycle
- `TenancyServiceProvider` (NOT the stub) - Registers services, commands, and bootstrappers
- `Tenant` (model) - Represents individual tenants with domains and databases
- `Domain` (model) - Maps domains
```

</details>
