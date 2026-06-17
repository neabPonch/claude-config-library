---
name: d-kuro__gwq
source: https://github.com/d-kuro/gwq/blob/c4247734968bc3f66addd1e088c19b962c27cfc1/CLAUDE.md
repo: d-kuro/gwq
kind: claude-md
stars: 428
last_pushed: 2026-05-02T04:42:24Z
license: apache-2.0
score: 8
domains: [cli-tools, go]
tags: [short, minimalist, context-efficient]
curated: 2026-06-14
curated_by: config-scout
---

# d-kuro/gwq — claude-md

**Why it's worth keeping:** The specific instruction to 'Keep this file under 20-30 lines' is a high-tier technique that forces the user to only include non-obvious, high-leverage intent and commands.

**Summary:** This file implements an extreme minimalism strategy designed to prevent context bloat in LLM windows.

**Source credibility:** High; derived from a popular Git tool with recent activity.

**Recency:** Very current; focuses on context management which is essential for Claude Code's token efficiency.

**Source:** [d-kuro/gwq/CLAUDE.md](https://github.com/d-kuro/gwq/blob/c4247734968bc3f66addd1e088c19b962c27cfc1/CLAUDE.md) · 428★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Agent Guidelines

## Core Principles

- **Do NOT maintain backward compatibility** unless explicitly requested. Break things boldly.
- **Keep this file under 20-30 lines of instructions.**

---

## Project Overview

**Project type:** CLI tool — Git worktree manager
**Primary language:** Go

---

## Commands

```bash
make build          # Build to ./gwq
make test           # go test ./...
make lint           # golangci-lint run
make install        # Build and install gwq
```

---

## Code Conventions

- Follow the existing patterns in the codebase
- Prefer explicit over clever
- Delete dead code immediately

---

## Maintenance Notes

**Keep this file lean and current:**

1. **Review regularly** - stale instructions poison the agent's context
2. **CRITICAL: Keep total under 20-30 lines** - move detailed docs to separate files and reference them
3. **Update commands immediately** when workflows change
4. **Delete anything the agent can infer** from your code
```

</details>
