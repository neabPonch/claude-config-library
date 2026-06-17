---
name: Triple1090__leine-honig
source: https://github.com/Triple1090/leine-honig/blob/3bbad27e66b4c38c876cf8340b3ae7230643ea42/CLAUDE.md
repo: Triple1090/leine-honig
kind: claude-md
stars: 0
last_pushed: 2026-05-23T14:46:48Z
license: unknown
score: 9
domains: [web-frontend, e-commerce, nextjs]
tags: [architecture, state-management, tailwind-v4, medusa-v2]
curated: 2026-06-15
curated_by: config-scout
---

# Triple1090/leine-honig — claude-md

**Why it's worth keeping:** It documents crucial procedural logic (checkout sequences), state management details (localStorage keys), and specific security/styling constraints that prevent AI errors.

**Summary:** Provides high-density architectural context for a Next.js e-commerce application integrated with Medusa v2.

**Source credibility:** Personal project repository with recent updates.

**Recency:** Highly current, explicitly referencing Tailwind CSS v4 and Media v2.

**Source:** [Triple1090/leine-honig/CLAUDE.md](https://github.com/Triple1090/leine-honig/blob/3bbad27e66b4c38c876cf8340b3ae7230643ea42/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

```bash
npm run dev      # Start development server at localhost:3000
npm run build    # Production build
npm run lint     # Run ESLint
```

No test suite is configured.

## Environment Variables

Copy `.env.example` to `.env.local` and fill in:

```
NEXT_PUBLIC_MEDUSA_BACKEND_URL=https://api.leine-honig.de   # or http://localhost:9000 for local dev
NEXT_PUBLIC_MEDUSA_PUBLISHABLE_KEY=your_publishable_key_here
```

## Architecture

This is a **Next.js app** (App Router, SSR enabled) for Leine-Honig, a honey shop. It is no longer a static export — server components fetch live data from a **Medusa v2 backend**.

**App Router structure** (`src/app/`):
- `layout.tsx` — Root layout: wraps all pages in `CartProvider`, renders Navbar, CartDrawer, and Footer
- `page.tsx` — Homepage: Hero → TrustBar → Welcome → Tes
- Shop flow: `/honig` (product listing) → `/honig/[handle]` (product detail with add-to-cart) → `/warenkorb` (cart review) → `/kasse` (checkout) → `/kasse/bestaetigung` (order confirmation)
- Other pages: `agb`, `bienen-mieten`, `datenschutz`, `impressu
```

</details>
