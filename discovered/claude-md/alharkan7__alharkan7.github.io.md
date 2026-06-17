---
name: alharkan7__alharkan7.github.io
source: https://github.com/alharkan7/alharkan7.github.io/blob/7550d69b68b9f34d847d49b942e501c4e542ee20/CLAUDE.md
repo: alharkan7/alharkan7.github.io
kind: claude-md
stars: 14
last_pushed: 2026-06-16T02:09:58Z
license: mit
score: 9
domains: [web-frontend, data-visualization]
tags: [astro, d3, mdx, static-site]
curated: 2026-06-16
curated_by: config-scout
---

# alharkan7/alharkan7.github.io — claude-md

**Why it's worth keeping:** Includes highly specific 'Four-Layer Architecture' instructions for its custom storytelling engine and explains the hybrid multi-framework component strategy. It also proactively clarifies the unique client-side authentication model to prevent incorrect architectural assumptions.

**Summary:** Detailed technical documentation for a specialized Astro-based static site featuring a custom D3 scrollytelling framework.

**Source credibility:** High quality; reflects a complex, well-structured personal project.

**Recency:** Extremely recent, referencing modern versions of Astro and pnpm.

**Source:** [alharkan7/alharkan7.github.io/CLAUDE.md](https://github.com/alharkan7/alharkan7.github.io/blob/7550d69b68b9f34d847d49b942e501c4e542ee20/CLAUDE.md) · 14★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a personal blog ([raihankalla.id](https://raihankalla.id)) built with Astro 5.16.6 as a static site for GitHub Pages deployment. The site uses a hybrid architecture combining Astro, React, and Svelte components with MDX for content authoring.

## Development Commands

```bash
# Install dependencies (requires pnpm)
pnpm install

# Start development server (runs on localhost:4321)
pnpm dev

# Build for production
pnpm build

# Preview production build
pnpm preview
```

**Important**: The `pnpm build` command runs a post-build script (`scripts/replace-redirect-pages.js`) that enhances redirect pages with custom templates.

## Architecture

### Static Site Strategy
- **Output Mode**: Static (`output: 'static'` in `astro.config.mjs`)
- **Deployment**: GitHub Pages (primary) and Vercel
- **Authentication**: Fully client-side Firebase Auth (no server-side endpoints required)
- **Content**: MDX files with frontmatter stored in `/src/posts/`

### Directory Structure

```
src/
├── components/          # Reusable UI components (Astro, React, Svelte)
```

</details>
