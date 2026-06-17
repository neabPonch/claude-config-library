---
name: DudeUnoob__dam-events
source: https://github.com/DudeUnoob/dam-events/blob/d910ef0e3c0c29bd73905dfa954a976c7273267c/claude.md
repo: DudeUnoob/dam-events
kind: claude-md
stars: 0
last_pushed: 2025-12-08T05:11:35Z
license: unknown
score: 9
domains: [web-frontend, fullstack-development, database-management]
tags: [nextjs, supabase, documentation-template]
curated: 2026-06-16
curated_by: config-scout
---

# DudeUnoob/dam-events — claude-md

**Why it's worth keeping:** The inclusion of an explicit file tree and detailed database schema provides essential high-density context to prevent AI structural hallucinations. It also uses concrete code examples to enforce specific coding standards and error handling patterns.

**Summary:** A comprehensive development guide for a Next.js/Supabase marketplace that maps out architecture, directory structures, and database schemas.

**Source credibility:** Low social proof (0 stars) but exhibits highly professional, structured technical documentation.

**Recency:** Current; uses modern Next.js 14 App Router paradigms.

**Source:** [DudeUnoob/dam-events/claude.md](https://github.com/DudeUnoob/dam-events/blob/d910ef0e3c0c29bd73905dfa954a976c7273267c/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# DAM Event Management Platform - Development Guide

## Project Overview

**Product Name:** DAM Event Platform  
**Version:** 1.0 - MVP (P0)  
**Tech Stack:** Next.js 14, React, Tailwind CSS, Supabase (PostgreSQL), TypeScript  
**Deployment:** Vercel  

**Purpose:** A two-sided marketplace connecting event planners (primarily student organizations) with pre-vetted vendors offering complete event packages (venue + catering + entertainment). We eliminate the fragmented vendor discovery process by centralizing package browsing, quote requests, and vendor communication.

---

## Core Architecture

```
Client (Next.js/React/Tailwind) 
  ↓ HTTPS
API Routes (Next.js Serverless)
  ↓
Supabase (PostgreSQL + Auth + Storage + Realtime)
  ↓
External APIs (Twilio, SendGrid, Google Maps)
```

### Key Technologies

| Component | Technology | Why |
|-----------|-----------|-----|
| Frontend | Next.js 14 + React 18 | SSR for SEO, unified front/back |
| Styling | Tailwind CSS | Rapid development, consistent design |
| Database | Supabase PostgreSQL | Open-source, RLS, realtime |
| Auth | Supabase Auth (Google OAuth) | Built-in OAuth, JWT, no passwords |
| Storage | Supabase Storage | S3-compatible, i
```

</details>
