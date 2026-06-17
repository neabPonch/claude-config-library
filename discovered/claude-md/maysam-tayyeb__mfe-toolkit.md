---
name: maysam-tayyeb__mfe-toolkit
source: https://github.com/maysam-tayyeb/mfe-toolkit/blob/c3730bb8820cd684869f780d5d7c041691554d03/claude.md
repo: maysam-tayyeb/mfe-toolkit
kind: claude-md
stars: 1
last_pushed: 2025-09-03T05:45:15Z
license: mit
score: 8
domains: [web-frontend, monorepo]
tags: [hierarchy, microfrontends, architecture]
curated: 2026-06-14
curated_by: config-scout
---

# maysam-tayyeb/mfe-toolkit — claude-md

**Why it's worth keeping:** The pattern of using nested CLAUDE.md files for specific domains and the use of 'CRITICAL' guardrails to prevent architectural drift are highly transferable techniques.

**Summary:** A sophisticated monorepo configuration that utilizes a hierarchical structure to distribute specialized context across subdirectories.

**Source credibility:** Low star count suggests a niche or personal project, but the structure is professionally documented.

**Recency:** Current; hierarchical context management is a vital pattern for modern large-scale AI coding.

**Source:** [maysam-tayyeb/mfe-toolkit/claude.md](https://github.com/maysam-tayyeb/mfe-toolkit/blob/c3730bb8820cd684869f780d5d7c041691554d03/claude.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides essential guidance to Claude Code when working with this MFE toolkit monorepo.

**Note**: Context-specific CLAUDE.md files exist in subdirectories for detailed guidance:
- `packages/CLAUDE.md` - Package development guidelines
- `apps/CLAUDE.md` - Application and MFE guidelines
- `packages/design-system/CLAUDE.md` - Design system rules (CRITICAL)
- Individual package/app directories may have their own CLAUDE.md files

## Essential Commands

### Development

```bash
# Install dependencies (run after cloning)
pnpm install

# Build packages and MFEs (required before first run)
pnpm build

# Start container application
pnpm dev:container-react  # React container app on http://localhost:3000

# Serve MFEs (in another terminal)
pnpm serve  # Serves from dist/ on http://localhost:8080
```

### Testing

```bash
# Run tests for all packages
pnpm test:packages

# Run tests for container app
pnpm test:container

# Run tests for a specific package
pnpm --filter @mfe-toolkit/core test
pnpm --filter @mfe/container-react test

# Watch mode for specific package tests
pnpm --filter @mfe/container-react test:watch

# Coverage report for specific package
pnpm --filter @
```

</details>
