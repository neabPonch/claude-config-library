---
name: mhenrixon__sidekiq-unique-jobs
source: https://github.com/mhenrixon/sidekiq-unique-jobs/blob/76aa8c947b8318ebbc5fa021be240097d7a926b3/CLAUDE.md
repo: mhenrixon/sidekiq-unique-jobs
kind: claude-md
stars: 1539
last_pushed: 2026-06-09T18:43:03Z
license: mit
score: 9
domains: [backend, distributed-systems, ruby]
tags: [middleware, redis, sidekiq]
curated: 2026-06-15
curated_by: config-scout
---

# mhenrixon/sidekiq-unique-jobs — claude-md

**Why it's worth keeping:** The 'Common Pitfalls' and 'Important Patterns' sections are elite; they provide the exact context an AI needs to avoid breaking subtle distributed system logic.

**Summary:** A comprehensive technical guide that explains complex architectural decisions like lock strategies, Lua script atomicity, and middleware ordering.

**Source credibility:** High-quality source: a widely used, well-maintained Ruby gem with significant GitHub popularity.

**Recency:** Very current; reflects modern development workflows including appraisal and specific Sidekiq integration details.

**Source:** [mhenrixon/sidekiq-unique-jobs/CLAUDE.md](https://github.com/mhenrixon/sidekiq-unique-jobs/blob/76aa8c947b8318ebbc5fa021be240097d7a926b3/CLAUDE.md) · 1539★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

sidekiq-unique-jobs is a Sidekiq middleware gem that prevents duplicate jobs from being enqueued or executed. It provides sophisticated locking mechanisms using Redis to ensure job uniqueness based on configurable parameters.

## Development Commands

### Testing
```bash
# Run all tests
bundle exec rspec

# Run specific test file
bundle exec rspec spec/path/to/spec.rb

# Run specific test by line number
bundle exec rspec spec/path/to/spec.rb:42

# Run tests with specific appraisals (different Sidekiq versions)
bundle exec appraisal rspec
bundle exec appraisal sidekiq-6.0 rspec
```

### Code Quality
```bash
# Run rubocop linter
bundle exec rake rubocop

# Run reek (code smell detector)
bundle exec rake reek

# Run all style checks
bundle exec rake style

# Generate documentation
bundle exec rake yard
```

### Build and Release
```bash
# Run all checks (style, tests, documentation)
bundle exec rake

# Release a new gem version (only for maintainers)
bundle exec rake release
```

## Architecture

### Lock Types

The gem implements multiple lock stra
```

</details>
