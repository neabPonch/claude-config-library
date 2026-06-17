---
name: KidsCollab__KidsCollab
source: https://github.com/KidsCollab/KidsCollab/blob/e87fa66d0c779cba4b080fa1764b0c1fd92eae36/CLAUDE.md
repo: KidsCollab/KidsCollab
kind: claude-md
stars: 1
last_pushed: 2026-04-04T11:09:50Z
license: mit
score: 8
domains: [web-frontend, static-site-generator]
tags: [quartz, documentation, architectural-patterns]
curated: 2026-06-16
curated_by: config-scout
---

# KidsCollab/KidsCollab — claude-md

**Why it's worth keeping:** Includes highly specific procedural rules (like the version bumping requirement) and maps logic/pipeline stages to directory structures rather than just listing files.

**Summary:** Provides deep architectural context for a plugin-based static site generator and clear command mappings.

**Source credibility:** Low star count, likely a solo developer project with high internal documentation quality.

**Recency:** Current; reflects modern ESM/TypeScript workflows.

**Source:** [KidsCollab/KidsCollab/CLAUDE.md](https://github.com/KidsCollab/KidsCollab/blob/e87fa66d0c779cba4b080fa1764b0c1fd92eae36/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a **Quartz 4.0** static site generator project used to build the KidsCollab website (migrating from Google Sites). It converts Obsidian-style Markdown notes into a full website with graph view, search, dark mode, popover previews, and more.

## Key Commands

- **`npx quartz build --serve`** — Build and serve the site locally (default content dir)
- **`npx quartz build --serve -d docs`** — Build and serve the docs folder specifically
- **`npx quartz build`** — Production build (outputs to `public/`)
- **`npm test`** — Run unit tests (path utilities + depgraph)
- **`npm run check`** — Type-check with TypeScript and run Prettier check
- **`npm run format`** — Format code with Prettier

## Architecture

Quartz uses a plugin-based content processing pipeline:

1. **Transformers** — Parse and transform Markdown content (frontmatter, links, LaTeX, syntax highlighting, table of contents, Obsidian/GitHub-flavored Markdown)
2. **Filters** — Include/exclude pages (e.g., `RemoveDrafts` filters pages marked as drafts)
3. **Emitters** — Generate output
```

</details>
