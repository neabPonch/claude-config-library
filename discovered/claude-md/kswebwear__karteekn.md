---
name: kswebwear__karteekn
source: https://github.com/kswebwear/karteekn/blob/bc5aa93f53fea394192bf728d8087ac5b57be98e/claude.md
repo: kswebwear/karteekn
kind: claude-md
stars: 0
last_pushed: 2026-04-19T14:44:53Z
license: unknown
score: 8
domains: [web-frontend, nextjs, content-management]
tags: [nextjs, ghost-cms, context-injection, typescript]
curated: 2026-06-14
curated_by: config-scout
---

# kswebwear/karteekn — claude-md

**Why it's worth keeping:** The 'Knowledge Base' startup routine is an advanced technique for injecting context without manual prompting; providing specific API endpoints prevents hallucination during data fetching tasks.

**Summary:** A structured guide for a Next.js and Ghost CMS project that emphasizes technical constraints and architectural patterns.

**Source credibility:** Low star count, but the highly structured content reflects a professional engineer's approach to documentation.

**Recency:** Current, utilizing modern Next.js 14 patterns and App Router logic.

**Source:** [kswebwear/karteekn/claude.md](https://github.com/kswebwear/karteekn/blob/bc5aa93f53fea394192bf728d8087ac5b57be98e/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Code Instructions

## Knowledge Base
Path: ~/second-brain/wiki
At session start:
1. Read wiki/hot.md
2. Read wiki/index.md  
3. Pull relevant domain pages before asking me for context
My decisions, patterns, bugs solved, and preferences are there.

## Project
Custom Next.js frontend for karteekn.com — a personal brand & technical blog by Karteek (ServiceNow Architect, 14+ years experience). Ghost CMS powers the content via headless API.

## Stack
- **Framework**: Next.js 14 (App Router)
- **Styling**: Tailwind CSS
- **CMS**: Ghost (headless, Content API)
- **Deploy**: Vercel
- **Images**: Nano Banana 2 (Google Gemini) — generated assets live in `/public/images/`
- **Language**: TypeScript

## Project Structure
```
/app              → App Router pages
/components       → Reusable UI components
/lib              → Ghost API client, utils, types
/public/images    → Nano Banana generated assets
/styles           → Global CSS + Tailwind config
```

## Key Rules
1. **Ghost API only** — never hardcode blog content; always fetch via `lib/ghost.ts`
2. **No inline styles** — Tailwind classes only
3. **Dark mode first** — use `dark:` variants; default theme is dark
4. **Mobile first*
```

</details>
