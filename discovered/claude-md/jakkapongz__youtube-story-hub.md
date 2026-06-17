---
name: jakkapongz__youtube-story-hub
source: https://github.com/jakkapongz/youtube-story-hub/blob/ba5e8b45b5572ca8ab950c18426710f3d44a2991/CLAUDE.MD
repo: jakkapongz/youtube-story-hub
kind: claude-md
stars: 0
last_pushed: 2026-02-07T15:09:22Z
license: unknown
score: 8
domains: [fullstack, web-frontend, data-pipeline]
tags: [context-heavy, status-tracking, directory-map]
curated: 2026-06-15
curated_by: config-scout
---

# jakkapongz/youtube-story-hub — claude-md

**Why it's worth keeping:** The 'Implementation Status' section is a high-value pattern; it prevents the AI from re-implementing existing logic by clearly defining what is 'Done'.

**Summary:** Provides an exhaustive technical overview including a complete file tree and a detailed progress checklist. It acts as a source of truth for both architecture and current development state.

**Source credibility:** Single-developer project, but contains highly detailed, structured documentation indicative of an active professional build.

**Recency:** Very recent (4 months ago) and includes cutting-edge tech like Next.js 15 and Tailwind v4.

**Source:** [jakkapongz/youtube-story-hub/CLAUDE.MD](https://github.com/jakkapongz/youtube-story-hub/blob/ba5e8b45b5572ca8ab950c18426710f3d44a2991/CLAUDE.MD) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# YouTube Story Hub - Project Context

## Project Overview

**Project Name:** YouTube Story Hub
**Brand Name:** หาเรื่องผี.com (Find Ghost Stories)
**Domain:** haruengphee.com
**Type:** AI-Powered YouTube Playlist Curation Platform
**Purpose:** Automatically curate and organize YouTube videos into smart playlists using AI
**Focus:** Thai ghost stories and paranormal content

---

## Tech Stack

```
Frontend: Next.js 15 (App Router, React 19, TypeScript)
Backend: Next.js API Routes
Database: PostgreSQL (Supabase) + Prisma 7 ORM
Styling: Tailwind CSS v4 (@theme inline)
Icons: Lucide React
Toast: react-hot-toast
Theme: next-themes (dark/light mode)
Data Collector: Python (SQLAlchemy + youtube-transcript-api)
AI: Claude API (planned)
Queue: BullMQ (planned)
Hosting: Vercel (deployed)
```

---

## Project Structure

```
haruengphee-web/              # Next.js frontend (renamed from web/)
├── src/
│   ├── app/
│   │   ├── page.tsx          # Public homepage (search form)
│   │   ├── layout.tsx        # Root layout with ThemeProvider
│   │   ├── globals.css       # Theme variables (dark/light + admin)
│   │   ├── sitemap.ts        # Dynamic sitemap for SEO
│   │   ├── robots.ts         #
```

</details>
