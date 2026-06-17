---
name: mostbyte__auth
source: https://github.com/mostbyte/auth/blob/5150a97d6c5da396e23369a847db0bbb6e3d3f3e/CLAUDE.md
repo: mostbyte/auth
kind: claude-md
stars: 0
last_pushed: 2026-01-27T10:16:44Z
license: mit
score: 8
domains: [backend, php-laravel, security]
tags: [architecture-flow, middleware, package-development]
curated: 2026-06-15
curated_by: config-scout
---

# mostbyte/auth — claude-md

**Why it's worth keeping:** The step-by-step 'Authentication Flow' explains how logic moves between files, which is vital for understanding complex middleware; it also includes specific Git/Tagging rules to prevent procedural errors.

**Summary:** Provides a clear architectural lifecycle and component map for a Laravel authentication package.

**Source credibility:** Low star count indicates a niche or new repo, but the documentation structure is professional and highly usable.

**Recency:** Extremely current, referencing PHP 8.4 and Laravel 12.

**Source:** [mostbyte/auth/CLAUDE.md](https://github.com/mostbyte/auth/blob/5150a97d6c5da396e23369a847db0bbb6e3d3f3e/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Mostbyte Auth is a PHP Laravel authentication package that integrates with an external identity service API. It provides authentication middleware and user model system for Laravel applications.

- **Language:** PHP 8.4+
- **Framework:** Laravel 11.x / 12.x
- **Purpose:** Token-based authentication via external identity service

## Common Commands

```bash
# Run tests
vendor/bin/phpunit

# Run a single test
vendor/bin/phpunit --filter testMethodName

# Install dependencies
composer install

# Publish config to consuming Laravel app
php artisan vendor:publish --provider="Mostbyte\Auth\AuthServiceProvider"
```

## Architecture

### Authentication Flow

1. **Request** → HTTP request with `Authorization: Bearer <token>` header
2. **IdentityAuth Middleware** → Extracts token, validates via `LoginUser::prepareAttributesForLogin()`
3. **Identity Service Client** → Makes HTTP request to `IDENTITY_BASE_URL/api/v1/auth/check-token`
4. **Cache Layer** → Caches user/token with TTL (2 hours default), key includes company + IP + device-id
5. **User Model** → C
```

</details>
