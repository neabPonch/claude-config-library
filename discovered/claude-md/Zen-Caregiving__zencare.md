---
name: Zen-Caregiving__zencare
source: https://github.com/Zen-Caregiving/zencare/blob/44c9aea4c8a58d042c586ba6ce5cec3976cf75e2/CLAUDE.md
repo: Zen-Caregiving/zencare
kind: claude-md
stars: 0
last_pushed: 2026-03-18T17:45:41Z
license: unknown
score: 8
domains: [web-frontend, backend-api, devops]
tags: [supabase, vanilla-js, deployment-guide]
curated: 2026-06-16
curated_by: config-scout
---

# Zen-Caregiving/zencare — claude-md

**Why it's worth keeping:** Includes explicit command sequences for multi-step deployments and clear 'post-deploy verification' checklists that an agent can use to confirm success.

**Summary:** A highly practical operational manual for a Supabase-backed Vanilla JS application covering local dev, deployment sequences, and verification.

**Source credibility:** Individual project with low social proof but high technical density.

**Recency:** Current; utilizes modern Supabase, Edge Functions, and Deno workflows.

**Source:** [Zen-Caregiving/zencare/CLAUDE.md](https://github.com/Zen-Caregiving/zencare/blob/44c9aea4c8a58d042c586ba6ce5cec3976cf75e2/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Zencare Volunteer Shift Tracker

## Stack
- Vanilla JS SPA (no build tools)
- Supabase (PostgreSQL + Auth + RLS + Edge Functions + pg_cron)
- GitHub Pages hosting
- Resend for email notifications

## Local Development
```bash
supabase start          # Start local Supabase stack
supabase db reset       # Apply migrations + seed data
python3 -m http.server 3000  # Serve locally at http://127.0.0.1:3000
```

## Key Ports
- Supabase API: 54321
- PostgreSQL: 54322
- Studio: 54323 (http://127.0.0.1:54323)
- Inbucket: 54324 (http://127.0.0.1:54324)

## Database
- Schema: `sql/001_schema.sql`
- Seed data: `sql/002_seed_data.sql`
- Migrations: `supabase/migrations/`
- Migration script: `scripts/import_spreadsheet.py`

## Edge Functions
- `supabase/functions/update-email/` - Email verification flow (sends verification email)
- `supabase/functions/verify-email/` - Handles verification link clicks (returns HTML)
- `supabase/functions/away-alert/` - Emails preferred volunteers when someone marks away
- `supabase/functions/shift-reminder/` - Daily shift reminders (triggered by pg_cron)
- `supabase/functions/weekly-digest/` - Weekly schedule email (triggered by pg_cron)
- `supabase/functions/ca
```

</details>
