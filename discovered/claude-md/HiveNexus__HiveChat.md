---
name: HiveNexus__HiveChat
source: https://github.com/HiveNexus/HiveChat/blob/9d1e8ed614923dcf74414357e0fe53f66b016c0a/CLAUDE.md
repo: HiveNexus/HiveChat
kind: claude-md
stars: 1157
last_pushed: 2025-09-16T16:08:49Z
license: other
score: 8
domains: [web-frontend, fullstack, ai-integration]
tags: [nextjs, drizzle, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# HiveNexus/HiveChat — claude-md

**Why it's worth keeping:** The inclusion of specific seeding commands (db:seedProvider, etc.) and high-level table descriptions is excellent for giving an agent immediate context on how to populate and query the system. It clearly distinguishes between Server Action vs Client Component patterns used in the project.

**Summary:** Provides a comprehensive architectural blueprint including technology stack, directory mapping, and detailed database schema descriptions.

**Source credibility:** Strong; a highly-starred repository indicating a mature/popular project structure.

**Recency:** Very current, utilizing modern standards like Next.js 14 App Router and Drizzle ORM.

**Source:** [HiveNexus/HiveChat/CLAUDE.md](https://github.com/HiveNexus/HiveChat/blob/9d1e8ed614923dcf74414357e0fe53f66b016c0a/CLAUDE.md) · 1157★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

HiveChat is a team-oriented AI chat application designed for small and medium teams. It supports multiple AI models (DeepSeek, OpenAI, Claude, Gemini, etc.) with a comprehensive admin system for managing users, models, and integrations.

## Development Commands

### Core Development
- `npm run dev` - Start development server on port 3000
- `npm run build` - Build the application for production
- `npm run start` - Start production server on port 3000
- `npm run lint` - Run ESLint to check code quality

### Database Operations
- `npm run initdb` - Initialize/update database schema and seed data
- `npm run db:seedProvider` - Seed LLM providers
- `npm run db:seedModel` - Seed AI models
- `npm run db:seedBot` - Seed bot templates
- `npm run db:seedGroup` - Seed user groups

## Architecture

### Technology Stack
- **Framework**: Next.js 14 with App Router
- **Database**: PostgreSQL with Drizzle ORM
- **Authentication**: NextAuth.js v5 with multiple providers
- **UI**: Tailwind CSS with Ant Design components
- **State Management**: Zustand

### Key Dire
```

</details>
