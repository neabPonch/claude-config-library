---
name: plvo__create-faster__claude
source: https://github.com/plvo/create-faster/blob/56648fb3cb13b4f163a74df0295a68849ca066a9/.claude/CLAUDE.md
repo: plvo/create-faster
kind: claude-md
stars: 27
last_pushed: 2026-06-14T13:20:54Z
license: mit
score: 9
domains: [cli-tools, dev-tooling]
tags: [scaffolding, template-engine, metadata-driven]
curated: 2026-06-15
curated_by: config-scout
---

# plvo/create-faster — claude-md

**Why it's worth keeping:** It explains the non-obvious logic of template resolution via file suffixes and custom Handlebars helpers, which is crucial for AI to understand how to modify templates correctly.

**Summary:** Highly detailed documentation for a metadata-driven CLI scaffolding tool that uses a single source of truth to manage complex project structures.

**Source credibility:** High; active, modern tool with clear architectural patterns.

**Recency:** Very current; utilizes Bun 1.2+ and TypeScript 5.9.

**Source:** [plvo/create-faster/.claude/CLAUDE.md](https://github.com/plvo/create-faster/blob/56648fb3cb13b4f163a74df0295a68849ca066a9/.claude/CLAUDE.md) · 27★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# create-faster - Project Documentation

Modern, type-safe CLI scaffolding tool for quickly creating production-ready projects with multiple framework combinations.

**Version**: 1.2.0
**Installation**: `bunx create-faster`
**License**: MIT

## Overview

CLI tool that generates full-stack projects with:
- **Interactive & Non-interactive modes**: Full interactive prompts or CLI flags for automation
- Interactive prompts with custom TUI (ASCII art, section headers, grouped multiselect)
- Multi-app support (automatic turborepo for 2+ apps)
- Modular system (Next.js: 10 modules, Expo: 1 module, Hono: 1 module)
- Package manager selection (bun/pnpm/npm + auto-install)
- Template engine with YAML frontmatter for path resolution and filtering
- **Auto-generated CLI command**: Copy-paste ready command to recreate projects

## Architecture

### Monorepo Structure
```
apps/cli/        # Main CLI (TypeScript + Bun)
apps/www/        # Docs website (Next.js - planned)
packages/config/ # Shared tsconfig
templates/       # Handlebars templates
```

### CLI Flow
1. Parse CLI flags (if provided) → 2. ASCII intro → 3. Interactive prompts (skipped if flags provided) → 4. Validation → 5. Template reso
```

</details>
