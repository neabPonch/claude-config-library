---
name: baomidou__mybatis-plus-doc
source: https://github.com/baomidou/mybatis-plus-doc/blob/c6ae1012fdf30cc6c74473d9f31d7080a319b7e1/CLAUDE.md
repo: baomidou/mybatis-plus-doc
kind: claude-md
stars: 751
last_pushed: 2026-01-11T12:04:55Z
license: unknown
score: 8
domains: [documentation, web-frontend, localization]
tags: [astro, i18n, automation, starlight]
curated: 2026-06-15
curated_by: config-scout
---

# baomidou/mybatis-plus-doc — claude-md

**Why it's worth keeping:** It defines specific workflows for content updates (root language first) and documents custom CLI commands for the AI to use for automated tasks like translation.

**Summary:** Provides instructions for an Astro-based documentation site featuring a custom multi-language translation automation system.

**Source credibility:** High; official documentation repository for MyBatis-Plus with active maintenance.

**Recency:** Current; explicitly references claude.ai/code in the file header.

**Source:** [baomidou/mybatis-plus-doc/CLAUDE.md](https://github.com/baomidou/mybatis-plus-doc/blob/c6ae1012fdf30cc6c74473d9f31d7080a319b7e1/CLAUDE.md) · 751★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is the official documentation site for MyBatis-Plus, built with Astro and Starlight. The site supports multi-language documentation (Chinese, English, Japanese) with an integrated translation plugin.

## Development Commands

```bash
# Start development server
npm run dev
# or
npm start

# Build the site (includes type checking)
npm run build

# Preview the built site
npm run preview

# Check types only
astro check
```

## Translation System

The project includes a custom translation plugin located in `translation-plugin/`:

```bash
# Translate all content to all target languages
npm run translate

# Translate to specific language
npm run translate:en    # English
npm run translate:ja    # Japanese

# Dry run to check what would be translated
npm run translate:check

# Incremental translation (only changed files)
npm run translate:incremental

# Translate specific file
npm run translate:file
npm run translate:en:file
npm run translate:ja:file
```

Translation configuration is in `translation-plugin/config.json`. The plugin supports multiple
```

</details>
