---
name: tribou__tabvalet
source: https://github.com/tribou/tabvalet/blob/09cfe6b20c4fb4a093dafa8c7a8d955164fec453/CLAUDE.md
repo: tribou/tabvalet
kind: claude-md
stars: 0
last_pushed: 2026-05-31T16:47:28Z
license: mit
score: 8
domains: [web-extension, frontend]
tags: [index-pattern, tdd-enforcement, command-reference]
curated: 2026-06-15
curated_by: config-scout
---

# tribou/tabvalet — claude-md

**Why it's worth keeping:** Uses a 'Context Index' pattern to prevent token bloat by routing agents to specialized docs; mandates TDD for bug fixes to ensure code quality.

**Summary:** Acts as a high-level project index that provides immediate command references and enforces strict development protocols.

**Source credibility:** Single developer/small project with very recent activity.

**Recency:** Highly current, utilizing modern modular documentation patterns for agentic workflows.

**Source:** [tribou/tabvalet/CLAUDE.md](https://github.com/tribou/tabvalet/blob/09cfe6b20c4fb4a093dafa8c7a8d955164fec453/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
*Global rules, command reference, and index to all project context — the only file AI agents need to open first*

# TabValet Context

Welcome to the **TabValet: Pinned Vertical Tabs** Chrome Extension repository. This extension replicates premium pinned/normal divider, drag-to-pin, and navigated `/` separator reset behaviors (reminiscent of the Arc Browser layout) inside a native Google Chrome side panel.

---

## Command Reference

Use these standard commands to test and manage this extension:

| Command | Action |
| --- | --- |
| `npm test` | Runs the Vitest unit testing suite once. |
| `npm run test:watch` | Starts Vitest in interactive watch mode. |
| `npm run test:e2e` | Runs Playwright headful end-to-end integration tests. |
| `npm run test:e2e:ui` | Starts Playwright test runner UI for interactive debugging. |

---

## CRITICAL Rules

> [!IMPORTANT]
> The following rules are absolute and must be followed by all development agents:

1. **Git commits**: Single-line only using `git commit -m "..."`. No multiline messages, no heredoc, no `Co-Authored-By`. Prefer Conventional Commits style (e.g., `feat: ...`, `fix: ...`, `docs: ...`).
2. **Bash syntax checking**: Use `bashcheck`
```

</details>
