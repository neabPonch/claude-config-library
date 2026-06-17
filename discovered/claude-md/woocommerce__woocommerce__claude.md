---
name: woocommerce__woocommerce__claude
source: https://github.com/woocommerce/woocommerce/blob/e892b5fa1abaece653086961fc53a666ab1572a5/plugins/woocommerce/client/admin/CLAUDE.md
repo: woocommerce/woocommerce
kind: claude-md
stars: 10349
last_pushed: 2026-06-15T03:48:16Z
license: unknown
score: 9
domains: [web-frontend, react, typescript]
tags: [workflow-optimization, linting-safety, architectural-patterns]
curated: 2026-06-15
curated_by: config-scout
---

# woocommerce/woocommerce — claude-md

**Why it's worth keeping:** Crucially warns against mass linting to prevent massive PR diffs and outlines a 'data-first' workflow pattern essential for large-scale development.

**Summary:** Provides highly specific, file-level command patterns and strict architectural constraints for a complex React/TypeScript environment.

**Source credibility:** High; part of the industry-standard WooCommerce repository with active maintenance.

**Recency:** Current, referencing modern versions of React and TypeScript.

**Source:** [woocommerce/woocommerce/plugins/woocommerce/client/admin/CLAUDE.md](https://github.com/woocommerce/woocommerce/blob/e892b5fa1abaece653086961fc53a666ab1572a5/plugins/woocommerce/client/admin/CLAUDE.md) · 10349★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Code Documentation for WooCommerce Admin Client

**Scope**: React/TypeScript development, Jest testing, Webpack builds
**Location**: `plugins/woocommerce/client/admin`

**See also:**

- `../../CLAUDE.md` - PHP tests and plugin-level documentation
- `client/settings-payments/CLAUDE.md` - Settings Payments module patterns

## Quick Reference Commands

```bash
# Testing
pnpm run test:js                             # Run all tests
pnpm run test:js -- status-badge.test.tsx    # Specific file

# Linting (ONLY specific files)
npx eslint --fix path/to/file.tsx            # Fix specific file
npx eslint path/to/file.tsx                  # Check specific file
pnpm run ts:check                            # Type checking
markdownlint --fix path/to/file.md           # Lint markdown files

# Building
pnpm run build                               # Production build
```

## When to Use This Documentation

Use this doc when you need to:

- Run or write Jest tests for React components
- Lint JavaScript/TypeScript/SCSS code
- Build or watch the admin client bundle
- Understand the admin client architecture
- Troubleshoot test or build failures

For module-specific patterns (like settings-payme
```

</details>
