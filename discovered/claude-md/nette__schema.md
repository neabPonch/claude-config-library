---
name: nette__schema
source: https://github.com/nette/schema/blob/4f11630c6ab8047905d911f6a0aea23b291bc771/CLAUDE.md
repo: nette/schema
kind: claude-md
stars: 1009
last_pushed: 2026-04-06T20:52:58Z
license: other
score: 9
domains: [backend-library, php]
tags: [architecture-deep-dive, testing-standards, implementation-patterns]
curated: 2026-06-17
curated_by: config-scout
---

# nette/schema — claude-md

**Why it's worth keeping:** It includes highly actionable testing helpers, exact command-line flags for debugging, and clear 'Common Patterns' that serve as a blueprint for implementation.

**Summary:** This config provides deep architectural insights, including the specific three-phase processing logic and internal magic method behaviors.

**Source credibility:** High; Nette is a cornerstone PHP ecosystem component with significant community trust and active maintenance.

**Recency:** Current; references modern PHP features and recent library versions (v1.3.2+).

**Source:** [nette/schema/CLAUDE.md](https://github.com/nette/schema/blob/4f11630c6ab8047905d911f6a0aea23b291bc771/CLAUDE.md) · 1009★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**Nette Schema** is a validation and normalization library for data structures. It provides a fluent API for defining schemas and validating configuration files, API inputs, and other structured data.

- **Package:** nette/schema
- **PHP Support:** 8.1 - 8.5
- **Dependencies:** nette/utils ^4.0
- **Documentation:** https://doc.nette.org/schema

## Development Commands

### Testing

```bash
# Run all tests
composer run tester

# Run specific test file
vendor/bin/tester tests/Schema/Expect.structure.phpt -s

# Run tests in specific directory
vendor/bin/tester tests/Schema/ -s
```

The `-s` flag shows test output (useful for debugging).

### Static Analysis

```bash
# Run PHPStan (level 8)
composer run phpstan
```

### Code Quality

- All PHP files must include `declare(strict_types=1)`
- PHPStan level 8 static analysis is enforced
- Follow Nette Coding Standard (based on PSR-12)
- Use tabs for indentation
- Use single quotes for strings

## Architecture Overview

### Core Schema Interface

The library is built around the `Schema` interface with fou
```

</details>
