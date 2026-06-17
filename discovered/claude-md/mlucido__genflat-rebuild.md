---
name: mlucido__genflat-rebuild
source: https://github.com/mlucido/genflat-rebuild/blob/79d121e1fadd35e9eab5062f19a1f31ea5809dfa/CLAUDE.md
repo: mlucido/genflat-rebuild
kind: claude-md
stars: 0
last_pushed: 2026-03-25T04:57:27Z
license: unknown
score: 7
domains: [web-frontend, cms]
tags: [nextjs, payload-cms, architecture]
curated: 2026-06-14
curated_by: config-scout
---

# mlucido/genflat-rebuild — claude-md

**Why it's worth keeping:** Specifies strict client-editing constraints and design tokens that prevent the AI from breaking layout via the CMS.

**Summary:** Provides architectural boundaries between CMS content and layout structure using Next.js and Payload CMS.

**Source credibility:** Low; likely a personal project with no social proof or history.

**Recency:** Current, utilizing modern versions of Next.js and Payload CMS.

**Source:** [mlucido/genflat-rebuild/CLAUDE.md](https://github.com/mlucido/genflat-rebuild/blob/79d121e1fadd35e9eab5062f19a1f31ea5809dfa/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# GenFlat Rebuild — Project Instructions

## Project
Rebuilding genflat.com for GenFlat Holdings, Inc.
Reference live site: https://www.genflat.com

## Stack
- Next.js 14 (App Router, TypeScript, Tailwind CSS)
- Payload CMS v3 (runs inside Next.js, single repo/deploy)
- SQLite locally → PostgreSQL in production (Neon or Railway)
- Vercel for deployment

## Client CMS Requirements
The client needs to edit copy, images, videos, and news posts
without developer involvement. Everything editable is modeled
as a Payload Global or Collection field. Layout is never
directly exposed to the client.

## Key Pages
- `/` — Single-page marketing site (7 sections)
- `/news` — News listing + individual article pages
- `/investor-information` — Static investor page

## Payload Content Model
- Globals: HomePage, SiteSettings, InvestorPage
- Collections: NewsArticles, Media, Users

## Design Tokens
Dark navy/charcoal backgrounds, gold/amber accent, white text.
Montserrat Black for headings, Inter for body.
Client can adjust colors + fonts via SiteSettings global in admin.

## Conventions
- All components are TypeScript React Server Components unless interactivity required
- Use next/image for all ima
```

</details>
