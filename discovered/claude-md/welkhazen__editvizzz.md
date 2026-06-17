---
name: welkhazen__editvizzz
source: https://github.com/welkhazen/editvizzz/blob/b1401f02352f980d9c1d37b718a27c61ceaff9fa/claude.md
repo: welkhazen/editvizzz
kind: claude-md
stars: 0
last_pushed: 2026-03-14T03:36:07Z
license: unknown
score: 7
domains: [web-frontend, react]
tags: [react, typescript, supabase, tailwind]
curated: 2026-06-14
curated_by: config-scout
---

# welkhazen/editvizzz — claude-md

**Why it's worth keeping:** Includes an 'Important Notes' section that enforces critical constraints like not modifying UI primitives and explains unique domain rules (token economy).

**Summary:** Provides a comprehensive technical context for a React/Supabase application, including directory mappings and business logic.

**Source credibility:** Low social proof via GitHub stars, but contains highly specific project-level details.

**Recency:** Current; uses modern toolsets like Vite, React 18, and TanStack Query.

**Source:** [welkhazen/editvizzz/claude.md](https://github.com/welkhazen/editvizzz/blob/b1401f02352f980d9c1d37b718a27c61ceaff9fa/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Code - Project Context

## Project Overview

**The Art of raW** is a premium wellness/fitness instructor booking platform built with React, TypeScript, and modern web technologies. Users can browse instructors, book sessions (individual or group), manage tokens as currency, and track their wellness journey with gamification elements.

## Tech Stack

- **Framework**: React 18 + TypeScript
- **Build Tool**: Vite
- **Styling**: Tailwind CSS + shadcn/ui components
- **State Management**: React Query (TanStack Query)
- **Routing**: React Router v6
- **Animations**: Framer Motion
- **Backend**: Supabase (auth, database)
- **Forms**: React Hook Form + Zod validation

## Project Structure

```
src/
├── components/          # Shared UI components
│   ├── ui/              # shadcn/ui primitives (DO NOT EDIT directly)
│   ├── filters/         # Filter components for instructor search
│   ├── matching/        # User-instructor matching components
│   └── instructor-waitlist/  # Instructor onboarding flow
├── features/            # Feature-based page components
│   ├── home/            # HomePage
│   ├── instructors/     # InstructorProfilePage
│   ├── booking/         # BookingPage
│
```

</details>
