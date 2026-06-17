---
name: LakishaDev__vaga-beta-react__claude
source: https://github.com/LakishaDev/vaga-beta-react/blob/37e8f9f652cc6870344bd82c16a73314323b2c9b/.claude.design/usluge-design/uploads/CLAUDE.md
repo: LakishaDev/vaga-beta-react
kind: claude-md
stars: 0
last_pushed: 2026-05-11T18:05:25Z
license: mit
score: 9
domains: [web-frontend, fullstack-react, ssr-deployment]
tags: [react, vite, ssr, cloudflare, hybrid-architecture]
curated: 2026-06-16
curated_by: config-scout
---

# LakishaDev/vaga-beta-react — claude-md

**Why it's worth keeping:** It includes critical 'gotchas' for SSR safety, such as dependency management in vite.config.js and window access guards. The explicit breakdown of different entry points prevents the AI from breaking the hybrid deployment model.

**Summary:** A highly detailed guide for a hybrid SSR/CSR React application using Vite and Cloudflare. It explains how the project bifurcates into marketing and e-commerce logic.

**Source credibility:** Single developer repository; low social proof but contains high-density technical documentation.

**Recency:** Extremely current, mentioning React 19 and Vite 7.

**Source:** [LakishaDev/vaga-beta-react/.claude.design/usluge-design/uploads/CLAUDE.md](https://github.com/LakishaDev/vaga-beta-react/blob/37e8f9f652cc6870344bd82c16a73314323b2c9b/.claude.design/usluge-design/uploads/CLAUDE.md) · 0★

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
