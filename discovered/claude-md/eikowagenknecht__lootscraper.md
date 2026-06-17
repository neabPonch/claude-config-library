---
name: eikowagenknecht__lootscraper
source: https://github.com/eikowagenknecht/lootscraper/blob/641c5c460d1cba07bd191d4e252c3cef9d89f6c6/CLAUDE.md
repo: eikowagenknecht/lootscraper
kind: claude-md
stars: 291
last_pushed: 2026-05-25T07:41:51Z
license: mit
score: 9
domains: [web-scraping, backend-services, bot-development]
tags: [typescript, service-oriented, automation, scraper]
curated: 2026-06-15
curated_by: config-scout
---

# eikowagenknecht/lootscraper — claude-md

**Why it's worth keeping:** It explicitly distinguishes between unit and contract testing strategies and details the specific orchestration pattern used to initialize services.

**Summary:** A highly detailed guide for a service-oriented scraping application that covers command sets, architectural hierarchy, and data flow.

**Source credibility:** High; 291 stars and recent commits indicate an active, community-validated repository.

**Recency:** Very current, utilizing modern tooling like Node 22 and pnpm.

**Source:** [eikowagenknecht/lootscraper/CLAUDE.md](https://github.com/eikowagenknecht/lootscraper/blob/641c5c460d1cba07bd191d4e252c3cef9d89f6c6/CLAUDE.md) · 291★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

**Install dependencies:**
```bash
pnpm install
playwright install firefox  # Required for browser automation
```

**Development:**
```bash
pnpm run dev          # Run in development mode with debug logging
pnpm run build        # Build for production  
pnpm run start        # Run production build
```

**Testing:**
```bash
pnpm test             # Run unit tests
pnpm test:watch       # Run tests in watch mode
pnpm test:contract    # Run contract tests (integration tests with external APIs)
pnpm test:coverage    # Run tests with coverage report
pnpm test:all         # Run both unit and contract tests
```

**Linting and Type Checking:**
```bash
pnpm run lint         # Full lint (TypeScript check + oxlint + oxfmt)
pnpm run type-check   # TypeScript type checking only
pnpm run check        # Combined lint + type-check
pnpm run format       # Format code with oxfmt
```

**Docker:**
```bash
docker build . -t eikowagenknecht/lootscraper:develop
docker run --volume "${PWD}/data:/data" --name lootscraper eikowagenknecht/lootscraper:develop
```

## Archi
```

</details>
