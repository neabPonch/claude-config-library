---
name: bugzmanov__bookokrat
source: https://github.com/bugzmanov/bookokrat/blob/a14638b209a4b4e2b46dc2ea3f7bb5dd92f4f10d/CLAUDE.md
repo: bugzmanov/bookokrat
kind: claude-md
stars: 977
last_pushed: 2026-06-10T09:48:45Z
license: agpl-3.0
score: 9
domains: [cli-tools, systems-programming]
tags: [strict-instructions, data-persistence, performance]
curated: 2026-06-15
curated_by: config-scout
---

# bugzmanov/bookokrat — claude-md

**Why it's worth keeping:** Demonstrates how to use specific 'never/always' rules for sensitive areas like configuration management, serialization strategies, and environment-specific graphics protocols.

**Summary:** A highly prescriptive guide that enforces strict data integrity, backward compatibility, and specialized terminal rendering performance.

**Source credibility:** High; 977 stars and actively maintained repository.

**Recency:** Very current; tailored specifically for Claude Code workflows.

**Source:** [bugzmanov/bookokrat/CLAUDE.md](https://github.com/bugzmanov/bookokrat/blob/a14638b209a4b4e2b46dc2ea3f7bb5dd92f4f10d/CLAUDE.md) · 977★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## CRITICAL RULES FOR AI ASSISTANTS

0. **Working Directory**: NEVER CHANGE WORKING DIRECTORY UNLESS SPECIFICALLY ASKED. THE CURRENT USER WORKFLOW IS BASED ON WORKTREES, BY RECKLESSLY CHANGING DIRECTORIES YOU CAN MAKE IRREVERSIBLE DAMAGE.

1. **Testing**: ALWAYS use the existing SVG-based snapshot testing in `tests/svg_snapshots.rs`. NEVER introduce new testing frameworks or approaches.
1a. **Sandbox-Safe Tests**: All tests must run in sandboxed environments (e.g., Nix builds). This means tests MUST NOT: rely on a writable home directory or system directories (`dirs::data_dir()`, `dirs::cache_dir()`, etc.); make network requests; depend on system fonts, a real TTY, or specific environment variables (`TERM`, `COLORTERM`, `TERM_PROGRAM`); assume standard tools exist in `PATH` beyond what's declared as dependencies. Use `tempfile::TempDir` for any filesystem operations, and inject/mock any external dependencies rather than relying on the host environment.
2. **Golden Snapshots**: NEVER update golden snapshot files with `SNAPSHOTS=overwrite` unless explicitly requested b
```

</details>
