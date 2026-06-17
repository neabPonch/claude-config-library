---
name: sajor2000__clif_website
source: https://github.com/sajor2000/clif_website/blob/51bf49793f6a861cc2ed703cd1309d62ab1a0f75/CLAUDE.md
repo: sajor2000/clif_website
kind: claude-md
stars: 5
last_pushed: 2026-06-12T19:18:17Z
license: apache-2.0
score: 9
domains: [web-frontend, documentation]
tags: [astro, data-synchronization, workflow-instructions]
curated: 2026-06-15
curated_by: config-scout
---

# sajor2000/clif_website — claude-md

**Why it's worth keeping:** The 'Data Dictionary' section is a masterclass in providing exact, multi-step workflows for keeping SQL, Markdown, Astro, and JSON sources of truth in sync. It also includes highly specific rules for updating manual counters to prevent documentation drift.

**Summary:** This file provides deep architectural context and rigorous procedural instructions for maintaining data-driven consistency across multiple disparate files.

**Source credibility:** High; the repository is active and reflects a sophisticated data migration project.

**Recency:** Current; provides high-value procedural guardrails useful for modern agentic coding workflows.

**Source:** [sajor2000/clif_website/CLAUDE.md](https://github.com/sajor2000/clif_website/blob/51bf49793f6a861cc2ed703cd1309d62ab1a0f75/CLAUDE.md) · 5★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Security Rules

- **NEVER read, cat, or access `.env` files** — they contain secrets. Only read `.env.example`.
- If you need to know what env vars exist, check `.env.example` instead.

## Project Overview

This is the CLIF Consortium website - a healthcare consortium website built with Astro that showcases the Common Longitudinal ICU data Format standard for critical care data research. The project has been migrated from static markdown files to a modern Astro framework.

## Commands

### Development

```bash
npm run dev      # Start development server on http://localhost:4321
npm run build    # Build for production to ./dist
npm run preview  # Preview production build locally
npm run lint     # Run ESLint
npm run format   # Format code with Prettier
npm run typecheck # Run TypeScript type checking
npm test         # Run tests with Vitest
```

### Image Management

```bash
python download_png_images.py      # Download PNG images from markdown files
python test_png_references.py      # Verify PNG references in Astro files
python test_png_display.py         # Test
```

</details>
