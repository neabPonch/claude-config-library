---
name: metabase__metabase
source: https://github.com/metabase/metabase/blob/c1c9bb4f1c1ef35e4bd35b0f4297ed3872c69d2a/CLAUDE.md
repo: metabase/metabase
kind: claude-md
stars: 47688
last_pushed: 2026-06-15T17:19:09Z
license: other
score: 10
domains: [backend, clojure, monorepo, mcp-integration]
tags: [modular-skills, mcp, tool-specialization, test-automation]
curated: 2026-06-15
curated_by: config-scout
---

# metabase/metabase — claude-md

**Why it's worth keeping:** The 'Skill' pattern allows for extreme scalability in large codebases; the specific instruction to avoid progress-bar-heavy shell commands prevents the LLM from losing context due to messy output.

**Summary:** Implements a highly sophisticated modular architecture by delegating domain-specific instructions to specialized '.claude/skills/' sub-directories. It provides strict guidance on tool preferences and command execution to ensure high-quality, parseable agent feedback.

**Source credibility:** Very high; Metabase is a top-tier, widely used open-source project with active maintenance.

**Recency:** Highly current, specifically leveraging the modern MCP (Model Context Protocol) ecosystem.

**Source:** [metabase/metabase/CLAUDE.md](https://github.com/metabase/metabase/blob/c1c9bb4f1c1ef35e4bd35b0f4297ed3872c69d2a/CLAUDE.md) · 47688★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Metabase Development Guide

# Skills

For detailed guidance on writing and reviewing code and documentation, see the skills in [.claude/skills/](.claude/skills/):

## Clojure

### clojure-mcp tools

- **[clojure-eval](.claude/skills/clojure-eval/SKILL.md)** - Always use this to evaluate Clojure code, **run tests**, and verify edits/compile. Prefer this over shell commands.
- **[clojure-write](.claude/skills/clojure-write/SKILL.md)** - Clojure/ClojureScript development with REPL-driven workflow and coding conventions
- **[clojure-review](.claude/skills/clojure-review/SKILL.md)** - Clojure/ClojureScript code review guidelines and style enforcement

### clojure-mcp-lite tools

- **clj-nrepl-eval** - This is another good mechanism for running Clojure code on an nrepl server.

## TypeScript

- **[typescript-write](.claude/skills/typescript-write/SKILL.md)** - TypeScript/JavaScript development and best practices
- **[typescript-review](.claude/skills/typescript-review/SKILL.md)** - TypeScript/JavaScript code review guidelines

## Documentation

- **[docs-write](.claude/skills/docs-write/SKILL.md)** - Documentation writing with Metabase style guide
- **[docs-review](.claude/skills/docs-
```

</details>
