---
name: eyra__mono__claude
source: https://github.com/eyra/mono/blob/622bd6a8bf37e99ac017b298d1f175824950f63c/core/CLAUDE.md
repo: eyra/mono
kind: claude-md
stars: 11
last_pushed: 2026-06-14T21:43:29Z
license: agpl-3.0
score: 9
domains: [backend, devops, elixir-phoenix, infrastructure]
tags: [debugging-heuristics, infrastructure-quirks, deployment-checklists]
curated: 2026-06-15
curated_by: config-scout
---

# eyra/mono — claude-md

**Why it's worth keeping:** It includes high-level debugging heuristics ('Never Assume') and documents non-obvious infrastructure pitfalls like the specific S3 domain format required to avoid errors.

**Summary:** This file provides highly specific infrastructure knowledge for a Phoenix/Fly.io stack, including critical S3 configuration quirks and deployment checklists.

**Source credibility:** A small but active specialized mono-repo with recent activity.

**Recency:** Highly current; reflects modern cloud deployment workflows using Fly.io and Tigris.

**Source:** [eyra/mono/core/CLAUDE.md](https://github.com/eyra/mono/blob/622bd6a8bf37e99ac017b298d1f175824950f63c/core/CLAUDE.md) · 11★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## CRITICAL DEBUGGING PRINCIPLE

**NEVER ASSUME - ALWAYS INVESTIGATE**

Before attempting any fix:
1. **Trace the actual error** - Find where the error originates, not where you think it might be
2. **Verify data structures** - Check what data is actually being passed vs. what's expected
3. **Understand the context** - Know why there's a mismatch before proposing solutions
4. **Test your hypothesis** - Verify your understanding before making changes

Making changes based on assumptions without investigation leads to:
- Fixing the wrong problem
- Breaking other parts of the system
- Missing the real issue entirely

Always investigate first, understand second, fix third.

## Development Commands

### Setup and Dependencies
- `mix setup` - Full project setup (deps, database, assets)
- `mix deps.get` - Install Elixir dependencies
- `cd assets && npm install` - Install frontend dependencies

### Database
- `mix ecto.setup` - Create and migrate database
- `mix ecto.migrate` - Run database migrations
- `mix ecto.reset` - Drop and recreate database
- `mix seed` - Run idempot
```

</details>
