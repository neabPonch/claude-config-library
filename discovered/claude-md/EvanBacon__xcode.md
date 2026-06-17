---
name: EvanBacon__xcode
source: https://github.com/EvanBacon/xcode/blob/1731d01f4e6bf5384b9d164714b609909d567acd/CLAUDE.md
repo: EvanBacon/xcode
kind: claude-md
stars: 218
last_pushed: 2026-06-09T18:04:05Z
license: unknown
score: 10
domains: [cli-tools, build-systems, typescript]
tags: [architecture, patterns, xcode]
curated: 2026-06-17
curated_by: config-scout
---

# EvanBacon/xcode — claude-md

**Why it's worth keeping:** It provides exact implementation requirements through code snippets to prevent logic errors. The 'Research' section includes a unique tip for handling difficult documentation formats.

**Summary:** Defines a TypeScript library for Xcode project parsing by detailing its dual-layer architecture and object management patterns.

**Source credibility:** High; well-maintained repository with significant star count.

**Recency:** Current; reflects modern development workflows and toolsets.

**Source:** [EvanBacon/xcode/CLAUDE.md](https://github.com/EvanBacon/xcode/blob/1731d01f4e6bf5384b9d164714b609909d567acd/CLAUDE.md) · 218★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

This is `@bacons/xcode`, a TypeScript package that provides a spec-compliant parser for Xcode's `.pbxproj` files (project files). It's designed as a faster, more accurate alternative to the legacy `xcode` npm package, using Chevrotain parser instead of PEG.js.

The package offers two main APIs:
1. **Low-level JSON API** (`src/json/`) - Direct parsing and building of pbxproj files
2. **High-level Object API** (`src/api/`) - Mutable graph-based API for easier manipulation

## Development Commands

- **Build**: `bun build` (compiles TypeScript to `build/` directory)
- **Test**: `bun test` (runs Jest tests)
- **Clean**: `bun clean` (removes build directory)
- **Test single file**: `bun test <filename>` (e.g., `bun test PBXProject.test.ts`)
- **Watch tests**: `bun test --watch`

## Architecture

### Core Components

**JSON Layer** (`src/json/`):
- `parser/` - Chevrotain-based parser for pbxproj format (old-style plist)
- `writer.ts` - Serializes JSON back to pbxproj format
- `types.ts` - TypeScript definitions for all pbxproj object types
- `unicode/` - Handl
```

</details>
