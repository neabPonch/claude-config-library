---
name: viclafouch__meme-studio
source: https://github.com/viclafouch/meme-studio/blob/d8fa0befde7069182525bfc5f5bac5c0c2c1c572/CLAUDE.md
repo: viclafouch/meme-studio
kind: claude-md
stars: 107
last_pushed: 2026-03-31T09:44:46Z
license: unknown
score: 9
domains: [web-frontend, agents-ai]
tags: [checklist-driven, plan-maintenance, agentic-workflow]
curated: 2026-06-15
curated_by: config-scout
---

# viclafouch/meme-studio — claude-md

**Why it's worth keeping:** The requirement to update '.claude/plan.md' mid-task prevents state drift, while the mandatory post-task checklist forces linting and 'simplification' workflows before completion is reported.

**Summary:** Establishes a rigorous agent lifecycle that mandates synchronization between code changes and an external plan file. It integrates custom command triggers for design and simplification to ensure high-quality outputs.

**Source credibility:** Reliable; shows evidence of a professional developer workflow with recent maintenance.

**Recency:** Extremely current, referencing React 19 and modern Next.js patterns.

**Source:** [viclafouch/meme-studio/CLAUDE.md](https://github.com/viclafouch/meme-studio/blob/d8fa0befde7069182525bfc5f5bac5c0c2c1c572/CLAUDE.md) · 107★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Meme Studio — a fast meme creation and customization tool. Users can pick from a default list of memes or import their own image, customize text, and download or share directly to Twitter. No server-side storage of user memes. Built with Next.js 16 (React 19, App Router).

The site is **bilingual FR/EN** (next-intl). Design is **mobile-first**, always responsive, and must work across all major browsers (Safari, Chrome, Firefox, etc.). Hosted on **Vercel**.

Website: [meme-studio.io](https://www.meme-studio.io)

## Tech Stack

- **Framework:** Next.js 16 (App Router, React 19)
- **Styling:** Panda CSS (build-time CSS-in-JS)
- **State:** Zustand + Immer
- **Async state:** TanStack Query
- **i18n:** next-intl
- **Icons:** FontAwesome
- **Validation:** Zod
- **Linting:** ESLint 9 (`@viclafouch/eslint-config-viclafouch`)
- **Formatting:** Prettier

## Commands

```bash
npm run build             # Production build (Next.js)
npm start                 # Start production server (port 8080)
npm run lint              # TypeScript check + ESLint
npm run lint
```

</details>
