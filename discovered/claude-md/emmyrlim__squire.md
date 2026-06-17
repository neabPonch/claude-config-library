---
name: emmyrlim__squire
source: https://github.com/emmyrlim/squire/blob/bfcb6761dfed02d09899a539feb9c186e54e838b/claude.md
repo: emmyrlim/squire
kind: claude-md
stars: 0
last_pushed: 2025-06-27T20:19:03Z
license: unknown
score: 8
domains: [fullstack, web-frontend, database-schema]
tags: [remix, supabase, shadcn, architecture]
curated: 2026-06-14
curated_by: config-scout
---

# emmyrlim/squire — claude-md

**Why it's worth keeping:** It documents specific SQL schemas, RLS query patterns (the 'two-step validation'), and exact UI component import paths that prevent the LLM from guessing file locations or logic.

**Summary:** Provides high-density architectural context for a full-stack Remix and Supabase application, focusing on complex data relationships and security patterns.

**Source credibility:** Low social proof via stars/activity, but contains highly professional architectural documentation.

**Recency:** Highly relevant as it uses current industry standards like Remix, Supabase, and shadcn/ui.

**Source:** [emmyrlim/squire/claude.md](https://github.com/emmyrlim/squire/blob/bfcb6761dfed02d09899a539feb9c186e54e838b/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Context - D&D Campaign Management App

## Project Overview

A web application for managing D&D campaigns, NPCs, quests, locations, and sessions. Built with modern web technologies and focused on user experience for dungeon masters.

For more details and product requirements, please read `docs/prd/product-requirements.md`. Update said product requirements document as necessary.

## Tech Stack

- **Framework**: Remix (React-based full-stack framework)
- **Database**: Supabase (PostgreSQL with real-time features)
- **Authentication**: Supabase Auth
- **Styling**: Tailwind CSS + shadcn/ui
- **Hosting**: Vercel
- **Language**: TypeScript

## Architecture Decisions

### URL Structure & Routing

- **User-scoped campaigns**: `/campaigns/{campaignSlug}` where slug is unique per user
- **Nested resources**: `/campaigns/{campaignSlug}/npcs/{npcSlug}`
- **Security**: All campaign resources are scoped to authenticated user via `created_by` field
- **Slugs**: Auto-generated from names, unique within scope (campaigns per user, NPCs per campaign)

### Database Schema Key Points

#### Core Tables

```sql
-- Users and Authentication
user_profiles (id) -> references auth.users(id)
  - displa
```

</details>
