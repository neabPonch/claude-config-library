---
name: BRO3886__ical
source: https://github.com/BRO3886/ical/blob/e0a7640c4d4be68517c3919c011f1e4104cf1137/CLAUDE.md
repo: BRO3886/ical
kind: claude-md
stars: 61
last_pushed: 2026-06-10T19:52:48Z
license: mit
score: 9
domains: [cli-tools, macos, go, agents-ai]
tags: [go, cli, macOS, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# BRO3886/ical — claude-md

**Why it's worth keeping:** It uses 'API trap prevention' by specifying exact methods for third-party libraries to prevent hallucinated usage, and includes crucial security/permission context for AI agent interaction.

**Summary:** Provides highly technical instructions for a Go-based macOS CLI, covering architecture, specific dependency API nuances, and domain-specific business logic.

**Source credibility:** High; a specialized, actively maintained tool (61 stars) with highly specific technical implementation details.

**Recency:** Current; mentions very recent dependency updates and modern AI 'skill' integration patterns.

**Source:** [BRO3886/ical/CLAUDE.md](https://github.com/BRO3886/ical/blob/e0a7640c4d4be68517c3919c011f1e4104cf1137/CLAUDE.md) · 61★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# ical — CLI for macOS Calendar

## Non-Negotiables
- **Conventional Commits**: ALL commits MUST follow [Conventional Commits](https://www.conventionalcommits.org/). Format: `type(scope): description`. Types: `feat`, `fix`, `docs`, `style`, `refactor`, `test`, `chore`, `build`, `ci`, `perf`. No exceptions.

## What is this?
Go CLI wrapping macOS Calendar via `go-eventkit`. Native EventKit bindings for 3000x faster reads than AppleScript. Single binary. Provides CRUD for events/calendars, natural language dates, recurrence rules, import/export, and multiple output formats.

**Repository**: `github.com/BRO3886/ical`

## Architecture
```
ical/
├── cmd/ical/
│   ├── main.go                  # Entry point (macOS check, version)
│   └── commands/                # Cobra CLI commands (one file per command)
│       ├── root.go              # Root cmd + global flags (--output, --no-color)
│       ├── calendars.go         # Calendar CRUD (list/create/update/delete subcommands)
│       ├── list.go              # List events (date range, filters)
│       ├── show.go              # Show single event detail
│       ├── add.go               # Create event (flags + interactive -i)
│       ├── updat
```

</details>
