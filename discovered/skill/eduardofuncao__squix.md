---
name: eduardofuncao__squix
source: https://github.com/eduardofuncao/squix/blob/8cb00f5eabb4a6d87155cd94cd47c5d785c86975/SKILL.md
repo: eduardofuncao/squix
kind: skill
stars: 240
last_pushed: 2026-06-12T21:55:02Z
license: mit
score: 9
domains: [cli-tools, database-management, sql]
tags: [sql, cli, automation]
curated: 2026-06-14
curated_by: config-scout
---

# eduardofuncao/squix — skill

**Why it's worth keeping:** Crucially lists 'Commands to Avoid' to prevent agent hang-ups in TUIs and emphasizes structured output formats (-f json) necessary for reliable data parsing.

**Summary:** Provides precise command mappings and operational constraints for using the Squix SQL CLI, specifically optimized for non-interactive AI agents.

**Source credibility:** A legitimate mid-sized open-source Go project with active maintenance.

**Recency:** Highly relevant; follows modern standards for making CLIs 'agent-friendly' by emphasizing non-interactive flows.

**Source:** [eduardofuncao/squix/SKILL.md](https://github.com/eduardofuncao/squix/blob/8cb00f5eabb4a6d87155cd94cd47c5d785c86975/SKILL.md) · 240★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Squix Skill for AI Coding Agents

## What is Squix

Squix is a CLI tool for managing and executing SQL queries across multiple
databases (PostgreSQL, MySQL, SQLite, Oracle, SQL Server, ClickHouse, Firebird).
It stores named queries in `~/.config/squix/config.yaml`.

## Critical Rules

1. **Always use `-f` with `squix run` for SELECT queries** — without it, SELECT results open an interactive TUI; non-SELECT queries print a status message either way
2. **No inline connection flag** — must `squix switch <name>` before queries
3. **Check connection first** — run `squix status` to verify reachability

## Non-Interactive Output

```bash
squix run <query> -f json        # JSON array of objects
squix run <query> -f csv         # CSV with header row
squix run <query> -f tsv         # Tab-separated values
squix run <query> -f markdown    # Markdown table
squix run <query> -f html        # HTML table with styling
squix run <query> -f sql         # INSERT statements
squix run "SELECT 1" -f json     # Inline SQL works too
squix run --last -f csv          # Re-run last query
```

Output goes to stdout, errors to stderr. Exit code 1 on failure.
Pipe cleanly: `squix run list_users -f json > user
```

</details>
