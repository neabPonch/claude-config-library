---
name: cathcoach4u__internal-coach4u-hub
source: https://github.com/cathcoach4u/internal-coach4u-hub/blob/09e6fda7c5a54cbe8fe0994e49ba82dc33b83f1b/CLAUDE.md
repo: cathcoach4u/internal-coach4u-hub
kind: claude-md
stars: 0
last_pushed: 2026-06-14T14:26:27Z
license: unknown
score: 9
domains: [web-frontend, workflow-automation]
tags: [session-handoff, context-management, developer-experience]
curated: 2026-06-14
curated_by: config-scout
---

# cathcoach4u/internal-coach4u-hub — claude-md

**Why it's worth keeping:** The 'Session Handoff' sequence prevents context drift in parallel environments, and the 'Working Preferences' for clickable links significantly reduces user friction during debugging/deployment.

**Summary:** Establishes a rigorous session handoff protocol that prioritizes state synchronization through specific file reading orders and database-driven tasks. It combines strict git workflows with human-centric interaction requirements.

**Source credibility:** Low public visibility (0 stars), likely an internal project for a specific professional use case.

**Recency:** Highly current; references modern stacks like Supabase, Edge Functions, and MCP-style workflows.

**Source:** [cathcoach4u/internal-coach4u-hub/CLAUDE.md](https://github.com/cathcoach4u/internal-coach4u-hub/blob/09e6fda7c5a54cbe8fe0994e49ba82dc33b83f1b/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Coach4U Internal Hub

## Session handoff — three things to read

Every new session reads these in order:
1. **`CHANGES.md`** — top 2-3 version entries, to see what just changed and any pending deploy/SQL.
2. **This file (`CLAUDE.md`)** — how the app is built + standing conventions.
3. **The `tasks` table** — **the single source of truth for outstanding items**, viewable in **Ops ▸
   Active Tasks** in the CRM or via SQL: `select id, title, priority, focus_date, work_category,
   description from tasks where status != 'Complete' and owner='cath' order by focus_date nulls last,
   priority desc;`. CHANGES.md no longer carries a separate "Outstanding" to-do block — that drift was
   removed in v3.65.246. To add/close work, write to the table (Active Tasks UI handles add/edit/done);
   don't reintroduce a markdown to-do anywhere.

Start/close-session prompts live in `docs/session-prompts.md` (and the in-app page `/session-prompts/`,
linked from the Home dashboard) — they encode the above flow.

**Two hard rules every session must follow:**
1. **Start of session:** `git fetch origin main && git reset --hard origin/main` — parallel sessions push
   here, so your local can be stale (e.g
```

</details>
