---
name: thedataquarry__thedataquarry.github.io
source: https://github.com/thedataquarry/thedataquarry.github.io/blob/10bfe8004f8bd29bb775368bb8fe278981a04d7c/CLAUDE.md
repo: thedataquarry/thedataquarry.github.io
kind: claude-md
stars: 5
last_pushed: 2026-04-30T14:09:25Z
license: apache-2.0
score: 9
domains: [web-frontend, static-site-generator]
tags: [astro, typescript, bun, shiki]
curated: 2026-06-15
curated_by: config-scout
---

# thedataquarry/thedataquarry.github.io — claude-md

**Why it's worth keeping:** The detailed documentation of path aliases and complex code-block transformers provides essential context that prevents the LLM from guessing how styles are applied.

**Summary:** Provides comprehensive technical context for an Astro/Bun static site, including deep-dive details on a custom Shiki syntax highlighting system.

**Source credibility:** Well-maintained technical blog with recent activity (2 months ago).

**Recency:** Highly current; utilizes modern tools like Astro 5.x and Bun.

**Source:** [thedataquarry/thedataquarry.github.io/CLAUDE.md](https://github.com/thedataquarry/thedataquarry.github.io/blob/10bfe8004f8bd29bb775368bb8fe278981a04d7c/CLAUDE.md) · 5★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

### Core Commands
```bash
# Development server with hot reload
bun dev
# or npm run dev

# Development server with type checking
bun dev:check

# Build the site
bun run build

# Preview built site
bun preview

# Type checking
bun check
# or astro check

# Linting and formatting
bun lint
bun format

# Create new blog post
bun new
# or astro-pure new

# Clean build artifacts
bun clean
```

## Architecture Overview

This is an Astro-based blog site using the "Pure" theme with TypeScript. The project follows a content-driven architecture optimized for technical blogging.

### Key Technologies
- **Astro 5.x**: Static site generator with component islands
- **TypeScript**: Full type safety throughout
- **UnoCSS**: Utility-first CSS framework with custom theme
- **astro-pure**: Custom theme package (located in `packages/pure/`)
- **Bun**: Primary package manager and task runner

### Project Structure
```
src/
├── components/        # Reusable Astro components
│   ├── about/        # About page specific components  
│   ├── home/         # Homepage c
```

</details>
