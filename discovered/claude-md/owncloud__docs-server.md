---
name: owncloud__docs-server
source: https://github.com/owncloud/docs-server/blob/6f4300306977d24bb6c0b8c264225d13542f8135/CLAUDE.md
repo: owncloud/docs-server
kind: claude-md
stars: 12
last_pushed: 2026-06-16T11:35:26Z
license: agpl-3.0
score: 8
domains: [documentation, static-site-generators]
tags: [antora, asciidoc, devops]
curated: 2026-06-16
curated_by: config-scout
---

# owncloud/docs-server — claude-md

**Why it's worth keeping:** The breakdown of file relationships (modules/partials/pages) and the explanation of custom build extensions are highly transferable for complex content repositories. It clearly distinguishes between production and local development workflows.

**Summary:** Provides technical context for an Antora-based documentation build system, covering module structure and global attribute injection.

**Source credibility:** High; comes from a major, actively maintained enterprise open-source project (ownCloud).

**Recency:** Current; provides all necessary context for modern developer-centric documentation workflows.

**Source:** [owncloud/docs-server/CLAUDE.md](https://github.com/owncloud/docs-server/blob/6f4300306977d24bb6c0b8c264225d13542f8135/CLAUDE.md) · 12★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

This is an [Antora](https://antora.org/)-based documentation site for ownCloud Server. Documentation is written in AsciiDoc and built into a static HTML site. This repo is not built standalone in production — it is built as part of the main [owncloud/docs](https://github.com/owncloud/docs) repository, but can be built locally for preview.

## Commands

Install dependencies:
```
npm install
```

Build documentation (production, fetches remote content and UI bundle):
```
npm run antora
```

Build for local preview (outputs to `public/`, served at `http://localhost:8080`):
```
npm run antora-dev-local
```

Serve the built site:
```
npm run serve
```

Build with a custom local UI bundle (from `../docs-ui/`):
```
npm run antora-dev-bundle
```

Check for broken links (run after build):
```
npm run linkcheck
```

## Architecture

### Content Structure

Content lives under `modules/`, organized into Antora modules:
- `modules/ROOT/` — Main landing pages and shared navigation
- `modules/admin_manual/` — Administration documentation
- `modules/developer_manual/` —
```

</details>
