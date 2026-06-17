---
name: LakishaDev__vaga-beta-react
source: https://github.com/LakishaDev/vaga-beta-react/blob/37e8f9f652cc6870344bd82c16a73314323b2c9b/CLAUDE.md
repo: LakishaDev/vaga-beta-react
kind: claude-md
stars: 0
last_pushed: 2026-05-11T18:05:25Z
license: mit
score: 9
domains: [web-frontend, ssr, cloud-infrastructure]
tags: [react, vite, cloudflare, hybrid-ssr, firebase]
curated: 2026-06-14
curated_by: config-scout
---

# LakishaDev/vaga-beta-react — claude-md

**Why it's worth keeping:** Excellent at detailing 'gotchas' like SSR-safe coding patterns, dependency externalization requirements, and specific shell syntax for environment variables.

**Summary:** Provides deep architectural context for a complex hybrid SSR-marketing and CSR-ecommerce setup using React 19 and Cloudflare.

**Source credibility:** Low star count suggests an individual developer project, but the technical depth of the documentation is high-tier.

**Recency:** Very current; explicitly mentions React 19 and Vite 7.

**Source:** [LakishaDev/vaga-beta-react/CLAUDE.md](https://github.com/LakishaDev/vaga-beta-react/blob/37e8f9f652cc6870344bd82c16a73314323b2c9b/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

Vaga Beta — React 19 + Vite 7 marketing site + e-commerce ("Prodavnica") for a Serbian scales/measuring-equipment company. Backed by Firebase (Auth, Firestore, Storage, App Check) and deployed to Cloudflare Pages with hybrid SSR (SSR for marketing pages, CSR for shop). User-facing copy is in Serbian.

## Common commands

```bash
npm run dev                # Vite dev server on :3000
npm run dev:ssr            # Express SSR dev server (server.js)
npm run lint               # ESLint over the repo
npm run build              # Client-only build (generates sitemap first)
npm run build:hybrid       # Client + SSR server bundle for Cloudflare
npm run build:cloudflare   # Full Cloudflare build incl. SEO smoke + sitemap
npm run deploy:cloudflare  # build:cloudflare + wrangler pages deploy
npm run preview:hybrid     # Local wrangler pages dev against dist/
npm run env:check          # Validate required VITE_* env vars
npm run seo:smoke:local    # SEO smoke test against local build
npm run seo:smoke:live     # SEO smoke test against production
npm run analyze
```

</details>
