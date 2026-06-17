---
name: ruby__www.ruby-lang.org
source: https://github.com/ruby/www.ruby-lang.org/blob/b7cf82d1edf20e80bc05819ad677c650ee5460e5/CLAUDE.md
repo: ruby/www.ruby-lang.org
kind: claude-md
stars: 940
last_pushed: 2026-06-04T23:47:47Z
license: unknown
score: 9
domains: [web-development, static-site]
tags: [jekyll, tailwind, multi-language, content-management]
curated: 2026-06-15
curated_by: config-scout
---

# ruby/www.ruby-lang.org — claude-md

**Why it's worth keeping:** Uses highly specific front-matter schemas and 'Important Conventions' to prevent common metadata/timezone errors; provides actionable CLI commands for routine tasks like localized news post generation.

**Summary:** A comprehensive operational guide for a complex, multi-lingual Jekyll site. It covers build processes, content creation workflows, and strict metadata standards.

**Source credibility:** High: official source code for the Ruby programming language website.

**Recency:** Current; reflects modern development workflows including Tailwind CSS.

**Source:** [ruby/www.ruby-lang.org/CLAUDE.md](https://github.com/ruby/www.ruby-lang.org/blob/b7cf82d1edf20e80bc05819ad677c650ee5460e5/CLAUDE.md) · 940★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is the Jekyll-based source for the official Ruby programming language website (www.ruby-lang.org), featuring multi-language support for 16+ languages and a Tailwind CSS-based design system.

## Build & Development Commands

### Jekyll Site Operations

```bash
# Build the site (takes several minutes)
bundle exec rake build

# Serve locally at http://localhost:4000/
bundle exec rake serve

# Alternative: Jekyll direct serve with incremental builds
bundle exec jekyll serve --watch --future --incremental
```

### CSS (Tailwind)

```bash
# Build CSS (production)
npm run build-css

# Watch CSS for development
npm run watch-css
```

### Testing & Quality Assurance

```bash
# Run all tests (includes linter, lint, build)
bundle exec rake test

# Run individual test suites
bundle exec rake test-news-plugin     # News archive plugin tests
bundle exec rake test-linter          # Linter library tests

# Linting
bundle exec rake lint                 # Markdown linter

# Post-build validation (requires built site)
bundle exec rake check:markup         # Va
```

</details>
