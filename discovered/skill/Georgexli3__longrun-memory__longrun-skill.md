---
name: Georgexli3__longrun-memory__longrun-skill
source: https://github.com/Georgexli3/longrun-memory/blob/1ffdd61655d7363e3d9c9755486d2c7e54a714f6/longrun-skill.md
repo: Georgexli3/longrun-memory
kind: skill
stars: 0
last_pushed: 2026-04-18T05:40:28Z
license: mit
score: 8
domains: [agents-ai, cli-tools]
tags: [memory-management, structured-knowledge]
curated: 2026-06-16
curated_by: config-scout
---

# Georgexli3/longrun-memory — skill

**Why it's worth keeping:** Uses high-signal knowledge categorization (kinds) and enforces a distinction between transient task logs and durable project invariants.

**Summary:** Provides a systematic workflow for using a CLI tool to maintain persistent, structured memory across ephemeral agent sessions.

**Source credibility:** Low social proof with 0 stars, but demonstrates sophisticated architectural patterns for agent state management.

**Recency:** Very current; updated within the last two months.

**Source:** [Georgexli3/longrun-memory/longrun-skill.md](https://github.com/Georgexli3/longrun-memory/blob/1ffdd61655d7363e3d9c9755486d2c7e54a714f6/longrun-skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: longrun-memory
description: Use when starting a task on a repo linked to longrun. Loads prior knowledge from persistent memory, records what this task learns, and tracks drift against the live code.
---

# Longrun Memory

You have persistent memory at `.memory/entries/`. It survives across sessions
and VMs; other agents write to the same store concurrently.

## Starting a task

Before making non-trivial changes, run:

```bash
longrun verify --quick                 # show stale/dead counts
longrun recall "<topic>"               # pull what others already learned
```

Read the top few hits. If any are `⚠ aging`, verify they're still accurate
against the live code before trusting them.

## During the task

You can search freely:

```bash
rg "<keyword>" .memory/entries/        # raw ripgrep, fastest
longrun recall "<query>" --kind project --limit 10
```

## Finishing a task

Write durable observations — not step-by-step task logs. Good memory is
things a future agent on a fresh VM would benefit from knowing.

```bash
longrun write --kind project \
  --refs path/to/file.ts::symbolName \
  --title "Short, searchable title" <<EOF
Body: why the code works the way it does, what in
```

</details>
