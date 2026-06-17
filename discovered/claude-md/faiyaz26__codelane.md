---
name: faiyaz26__codelane
source: https://github.com/faiyaz26/codelane/blob/1ccac7c0418b17342532ef32687644879aa78839/claude.md
repo: faiyaz26/codelane
kind: claude-md
stars: 18
last_pushed: 2026-03-27T11:28:38Z
license: agpl-3.0
score: 9
domains: [web-frontend, system-tools, rust, security]
tags: [comprehensive, negative-constraints, architecture-patterns]
curated: 2026-06-15
curated_by: config-scout
---

# faiyaz26/codelane — claude-md

**Why it's worth keeping:** Employs 'negative constraints' to prevent file bloat/documentation rot and provides specific code snippets for local API interactions. The 'Mandates' section creates highly actionable, non-negotiable rules for agentic workflows like version bumping.

**Summary:** A comprehensive project bible that combines high-level technical rationales with low-level operational mandates and code patterns.

**Source credibility:** Active repository with recent updates.

**Recency:** Extremely current; includes 2026 timestamps and modern tech stacks.

**Source:** [faiyaz26/codelane/claude.md](https://github.com/faiyaz26/codelane/blob/1ccac7c0418b17342532ef32687644879aa78839/claude.md) · 18★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Codelane Project Conventions

This document captures project-specific conventions, patterns, and decisions for future reference.

## Project Goals

Build a fast, efficient Agentic Development Environment that:
- Enables parallel feature development across multiple project "lanes"
- Provides AI agents with human-in-the-loop code review
- Integrates terminal, editor, and git interface
- Feels native and responsive
- Follows security best practices

## Mandates for AI Agents

1. **Release Notes**: When bumping versions or completing major features, MUST create/update `changelogs/v<VERSION>.md`. This is required for automated GitHub releases.
2. **Backend-Only Storage**: Lanes MUST be stored and managed by the Rust backend. Frontend MUST NOT have its own persistent lane store.
3. **Robust Command Execution**: 
   - Unix: Use interactive login shells (`-li`) to load user environments.
   - Windows: Wrap in `cmd /C` for batch/shim compatibility.
4. **Terminal Behavior**: Honor manual scrolling by pausing auto-scroll and showing a "Scroll to Bottom" button.

## Documentation Guidelines

**DO NOT create these types of files:**
- Implementation summaries (e.g., `IMPLEMENTATION_*.md`, `*_I
```

</details>
