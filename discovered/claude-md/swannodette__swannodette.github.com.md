---
name: swannodette__swannodette.github.com
source: https://github.com/swannodette/swannodette.github.com/blob/cd70f29f48fc3e5001f902ea3042e917f5e84690/CLAUDE.md
repo: swannodette/swannodette.github.com
kind: claude-md
stars: 82
last_pushed: 2026-01-24T17:17:50Z
license: unknown
score: 8
domains: [web-frontend, static-site, functional-programming]
tags: [jekyll, clojurescript, build-system, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# swannodette/swannodette.github.com — claude-md

**Why it's worth keeping:** It uses granular command lists (dev vs production builds) and explains complex architectural patterns that aren't obvious from code alone.

**Summary:** Provides highly specific build commands for Jekyll and various ClojureScript targets while explaining a unique interactive demo pattern.

**Source credibility:** High-quality documentation from a specialized personal project by an expert developer.

**Recency:** Very current; pushed within the last 5 months.

**Source:** [swannodette/swannodette.github.com/CLAUDE.md](https://github.com/swannodette/swannodette.github.com/blob/cd70f29f48fc3e5001f902ea3042e917f5e84690/CLAUDE.md) · 82★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is David Nolen's personal blog hosted at swannodette.github.com, built with Jekyll. The blog focuses on Lisp, Logic Programming, and JavaScript, with extensive ClojureScript examples and interactive demos.

## Common Development Commands

### Jekyll Site Development
- **Install dependencies**: `bundle install`
- **Start development server**: `rake preview` or `bundle exec jekyll serve --watch`
- **Build site**: `rake build` or `bundle exec jekyll build`
- **Create new blog post**: `rake post title="Post Title"` (optionally add `date="YYYY-MM-DD"`)
- **Create new page**: `rake page name="page-name.html"`

### ClojureScript Build Commands
Navigate to `code/blog/` directory for ClojureScript development:

- **Build all ClojureScript examples**: `lein cljsbuild once` (builds all configured targets)
- **Auto-rebuild during development**: `lein cljsbuild auto [build-id]`
- **REPL for development**: Use scripts in `code/blog/scripts/` directory

### Available ClojureScript Build Targets
Each example has both development and production builds:
-
```

</details>
