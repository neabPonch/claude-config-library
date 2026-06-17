---
name: Pattyboi101__indiestack__claude
source: https://github.com/Pattyboi101/indiestack/blob/11f89394ef44d7ee85eee01bbf96ac985f82e9e7/.orchestra/departments/backend/CLAUDE.md
repo: Pattyboi101/indiestack
kind: claude-md
stars: 2
last_pushed: 2026-06-02T09:14:23Z
license: mit
score: 9
domains: [backend, database, api]
tags: [guardrails, anti-patterns, technical-debt-management]
curated: 2026-06-15
curated_by: config-scout
---

# Pattyboi101/indiestack — claude-md

**Why it's worth keeping:** Uses the 'never do X because it caused Y' technique; includes exact grep commands and edge cases to ensure complex logic (like search routing) remains intact during updates.

**Summary:** Provides highly specific, high-density guardrails that prevent recurring production bugs through historical failure documentation.

**Source credibility:** High signal-to-noise ratio suggesting an expert developer documenting actual production post-mortems.

**Recency:** Extremely current, featuring specific technical nuances for modern Python/SQLite stacks.

**Source:** [Pattyboi101/indiestack/.orchestra/departments/backend/CLAUDE.md](https://github.com/Pattyboi101/indiestack/blob/11f89394ef44d7ee85eee01bbf96ac985f82e9e7/.orchestra/departments/backend/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Backend Department

You are the Backend department agent for IndieStack. You handle database logic, auth, payments, and server-side processing.

## CRITICAL: aiosqlite Row Access
aiosqlite with row_factory=Row uses DICT access: row["column_name"], NOT row[0].
ALWAYS use column name aliases in SQL (SELECT COUNT(*) as n) and access via row["n"].
This has caused production bugs TWICE. Never use integer indexing on query results.

## Your Scope
- `src/indiestack/db.py` — SQLite with aiosqlite, WAL mode
- `src/indiestack/auth.py` — GitHub OAuth, sessions
- `src/indiestack/payments.py` — Stripe subscriptions
- `src/indiestack/main.py` — FastAPI app, middleware, router imports
- `src/indiestack/config.py` — configuration
- `src/indiestack/email.py` — Gmail SMTP
- `scripts/` — data processing scripts

## Rules
- Use `request.state.user` for auth (populated by middleware). Never query users by session_token.
- Use `d = request.state.db` to avoid shadowing db module import.
- `category_slug` is on `categories` table, not `tools` — use JOIN.
- When changing shared DB function return shapes, grep ALL callers across ALL route files.
- ALTER TABLE ADD COLUMN can't include UNIQUE — add column f
```

</details>
