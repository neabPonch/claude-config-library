---
name: ChunPingWang__The_Art_of_Unit_Testing
source: https://github.com/ChunPingWang/The_Art_of_Unit_Testing/blob/18dfbb3c139d6b4ddc43f0e24f88c1bfa3cc4192/CLAUDE.md
repo: ChunPingWang/The_Art_of_Unit_Testing
kind: claude-md
stars: 0
last_pushed: 2025-12-20T16:29:31Z
license: mit
score: 7
domains: [testing, javascript, typescript]
tags: [unit-testing, jest, educational]
curated: 2026-06-15
curated_by: config-scout
---

# ChunPingWang/The_Art_of_Unit_Testing — claude-md

**Why it's worth keeping:** Explains a unique file-versioning convention (v1/v2) that prevents AI confusion and provides explicit shell commands for targeted testing.

**Summary:** Provides structured navigation for an educational repository and clear command patterns for running specific test files.

**Source credibility:** Educational codebase based on a recognized textbook; low star count but high structure quality.

**Recency:** 

**Source:** [ChunPingWang/The_Art_of_Unit_Testing/CLAUDE.md](https://github.com/ChunPingWang/The_Art_of_Unit_Testing/blob/18dfbb3c139d6b4ddc43f0e24f88c1bfa3cc4192/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Code samples for "The Art of Unit Testing, 3rd Edition" by Roy Osherove. This is an educational codebase demonstrating unit testing techniques, patterns, and frameworks using JavaScript and TypeScript.

## Commands

### Running Tests
```bash
npm test              # Run all Jest tests
npm run ch1           # Run chapter 1 custom test phases with linting
```

### Running a Single Test File
```bash
npx jest path/to/test.spec.js           # Run specific test file
npx jest --testPathPattern="pattern"    # Run tests matching pattern
```

## Codebase Structure

The repository is organized as chapter-by-chapter progression through unit testing concepts:

- **ch1-basics/** - Custom test runners from scratch (before frameworks)
- **ch2-first-test/** - Introduction to Jest testing framework
- **ch3-stubs/** - Replacing dependencies with stubs
- **ch4-mocks/** - Dependency injection patterns (parameter, modular, constructor, higher-order functions)
- **ch5-frameworks/** - Testing frameworks and faking libraries (Sinon, TestDouble)
- **ch6-async/** - Async te
```

</details>
