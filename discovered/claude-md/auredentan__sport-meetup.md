---
name: auredentan__sport-meetup
source: https://github.com/auredentan/sport-meetup/blob/921f2e6899417572344d954f28fa5da079cb2261/claude.md
repo: auredentan/sport-meetup
kind: claude-md
stars: 0
last_pushed: 2026-02-25T20:25:08Z
license: unknown
score: 9
domains: [web-frontend, fullstack-nextjs]
tags: [workflows, patterns, nextjs, typescript]
curated: 2026-06-14
curated_by: config-scout
---

# auredentan/sport-meetup — claude-md

**Why it's worth keeping:** The 'Common Tasks' section provides multi-file change sequences which prevent the AI from missing crucial updates, while the 'DO/DON'T' patterns enforce specific library usage rules.

**Summary:** A high-context guide that combines architectural constraints with explicit step-by-step workflows for feature implementation and API development.

**Source credibility:** Low visibility (0 stars) indicates a personal project, but the technical structure is professional and highly effective.

**Recency:** Very current; uses modern Next.js App Router and Drizzle ORM standards.

**Source:** [auredentan/sport-meetup/claude.md](https://github.com/auredentan/sport-meetup/blob/921f2e6899417572344d954f28fa5da079cb2261/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Development Guide - SportMeetup

This file contains important context and guidelines for AI assistants working on this project.

## Project Overview

SportMeetup is a web application for finding and organizing sports activities. Users can create activities, join existing ones, and manage their participation in various sports events.

**Tech Stack:**
- Next.js 16 (App Router)
- TypeScript
- SQLite with Drizzle ORM
- WorkOS for authentication
- Leaflet + OpenStreetMap for maps (free, no API key)
- Tailwind CSS for styling

## Architecture

### Database Schema

Located in `src/db/schema.ts`:

- **users**: User profiles from WorkOS
- **activities**: Sports activities with location coordinates
  - Supports recurring activities (daily, weekly, biweekly, monthly)
  - Stores `latitude` and `longitude` for map display
- **participants**: Join table linking users to activities

### Key Features

1. **Authentication**: WorkOS-based auth with session management
2. **Activity Management**: CRUD operations for activities
3. **Recurring Activities**: Support for repeating events
4. **Location Services**:
   - OpenStreetMap Nominatim for geocoding (free)
   - Leaflet for interactive maps
```

</details>
