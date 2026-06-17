---
name: mozilla-services__syncstorage-rs__skill
source: https://github.com/mozilla-services/syncstorage-rs/blob/b28317e972f40a982c792a743554c13abe1cd2b2/.claude/skills/multi-backend-consistency/SKILL.md
repo: mozilla-services/syncstorage-rs
kind: skill
stars: 1744
last_pushed: 2026-06-13T00:17:40Z
license: mpl-2.0
score: 9
domains: [backend-api, rust, database, devops]
tags: [trait-consistency, multi-db, rust-expert]
curated: 2026-06-15
curated_by: config-scout
---

# mozilla-services/syncstorage-rs — skill

**Why it's worth keeping:** The inclusion of Step 4 provides expert domain knowledge—such as transaction semantics and ID generation differences—transforming the agent from a syntax checker into a semantic auditor. The use of specific, actionable shell commands ensures the agent follows a predictable investigative workflow.

**Summary:** A highly specialized skill for ensuring Rust trait implementations remain consistent across multiple database backends (MySQL, Postgres, Spanner). It identifies both structural mismatches and subtle behavioral drift caused by database-specific logic.

**Source credibility:** High; based on a mature, well-maintained Mozilla repository with significant community traction.

**Recency:** 

**Source:** [mozilla-services/syncstorage-rs/.claude/skills/multi-backend-consistency/SKILL.md](https://github.com/mozilla-services/syncstorage-rs/blob/b28317e972f40a982c792a743554c13abe1cd2b2/.claude/skills/multi-backend-consistency/SKILL.md) · 1744★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: multi-backend-consistency
description: Checks that trait method changes in syncstorage-db or tokenserver-db are consistently implemented across all backend crates (mysql, postgres, spanner). Flags missing impls, behavioral drift, and Spanner-specific assumptions leaking into shared code.
user-invocable: true
---

# Multi-Backend Consistency Check

You are a Rust trait/implementation consistency reviewer for syncstorage-rs. Changes to shared traits must be reflected in every backend. Your job is to find gaps before they reach CI.

## Backend map

```
syncstorage-db/         ← trait definitions (DbPool, Db, etc.)
  → syncstorage-mysql/
  → syncstorage-postgres/
  → syncstorage-spanner/

tokenserver-db/         ← trait definitions
  → tokenserver-mysql/
  → tokenserver-postgres/
```

## Step 1 — Find changed trait files

```bash
git diff main...HEAD --name-only | grep -E "syncstorage-db/|tokenserver-db/"
```

If no trait files changed, check whether any backend implementation changed without a corresponding trait change — that may indicate the trait was bypassed or duplicated.

```bash
git diff main...HEAD --name-only | grep -E "syncstorage-(mysql|postgres|spanner)/|tokenser
```

</details>
