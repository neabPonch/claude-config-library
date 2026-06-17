---
name: zolplay-cn__website
source: https://github.com/zolplay-cn/website/blob/62166a952e558c06832b98300268525717f591ff/CLAUDE.md
repo: zolplay-cn/website
kind: claude-md
stars: 225
last_pushed: 2026-05-15T08:08:24Z
license: gpl-3.0
score: 7
domains: [web-frontend, nextjs]
tags: [nextjs, typescript, i18n, mdx]
curated: 2026-06-15
curated_by: config-scout
---

# zolplay-cn/website — claude-md

**Why it's worth keeping:** It highlights the non-standard content pattern (locale-specific MDX files) which prevents an LLM from misplacing page logic or structure.

**Summary:** Provides technical context for a Next.js 15 application utilizing MDX-based internationalization and server actions.

**Source credibility:** A real-world web project with moderate popularity and recent updates.

**Recency:** Highly current, referencing Next.js 15 and updated within the last month.

**Source:** [zolplay-cn/website/CLAUDE.md](https://github.com/zolplay-cn/website/blob/62166a952e558c06832b98300268525717f591ff/CLAUDE.md) · 225★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

This project uses pnpm as the package manager. Key commands:

- `pnpm dev` - Start development server on port 3333 with Turbo
- `pnpm build` - Build the production application
- `pnpm start` - Start production server
- `pnpm lint` - Run ESLint with Next.js configuration
- `pnpm lint:fix` - Format code with Prettier and fix linting issues
- `pnpm format` - Format code with Prettier
- `pnpm type-check` - Run TypeScript type checking without emitting files

## Architecture Overview

This is a Next.js 15 application using the App Router with internationalization support. Key architectural decisions:

### Framework Stack

- **Next.js 15** with App Router for routing and server-side rendering
- **TypeScript** for type safety
- **Tailwind CSS** for styling
- **next-intl** for internationalization (English and Chinese)
- **PostHog** for analytics with custom proxy configuration
- **Zod** for form validation and type safety

### Project Structure

- `app/[locale]/` - Internationalized pages using dynamic routing
- `modules/` - Feature-specific code (c
```

</details>
