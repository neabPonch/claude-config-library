---
name: Papr-ai__paprwork
source: https://github.com/Papr-ai/paprwork/blob/70f8dd1552ec44c59e0f3732e4042723db2b4388/CLAUDE.md
repo: Papr-ai/paprwork
kind: claude-md
stars: 6
last_pushed: 2026-06-13T17:31:00Z
license: agpl-3.0
score: 9
domains: [desktop-apps, electron, typescript, ai-agents]
tags: [architecture-patterns, environment-specs, coding-standards]
curated: 2026-06-15
curated_by: config-scout
---

# Papr-ai/paprwork — claude-md

**Why it's worth keeping:** It utilizes 'Decision Logs' to explain the rationale behind architecture, provides concrete code patterns for common tasks, and sets explicit limits on file sizes to enforce modularity.

**Summary:** This file provides high-fidelity architectural context, environment constraints (Node v24), and strict coding standards to prevent technical debt during a major rewrite.

**Source credibility:** High; includes specific, realistic toolchain details (oxlint/oxfmt) and version-specific requirements that demonstrate real-world engineering need.

**Recency:** Very current; references Node v24 and modern Rust-based web tooling.

**Source:** [Papr-ai/paprwork/CLAUDE.md](https://github.com/Papr-ai/paprwork/blob/70f8dd1552ec44c59e0f3732e4042723db2b4388/CLAUDE.md) · 6★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md - Project Context & Learnings

**Last Updated:** 2026-03-18

This file tracks key learnings, architectural decisions, and context for AI assistants working on Paprwork V2.

---

## Project Overview

**Paprwork V2** is a complete greenfield rewrite using OpenClaw's proven architecture:
- **Core App:** Electron + TypeScript (cross-platform: Mac, Windows, Linux)
- **Companion Apps:** Swift for native macOS/iOS features (future)
- **Dev Tools:** Rust-based tools for faster development
- **Local AI:** Ollama integration for on-device inference (privacy + zero cost)

**⚠️ CRITICAL: Node Version Requirement**
- **Requires Node v24+** (matches Electron 40's embedded Node v24.13.0)
- Use `nvm use 24` or `nvm install 24` before running any commands
- The `.nvmrc` file enforces this version
- `@electron/rebuild` requires Node v24+ features

**Quick Start:**
```bash
# 1. Switch to Node v24
nvm use 24

# 2. Install dependencies (auto-rebuilds native modules)
npm install

# 3. Start the app
npm start
```

**Why V2?**
- V1 accumulated 30,335 lines in monolithic files
- 90% code duplication between main + gateway processes
- Fragile with 10+ patches for tool calling issues
- No type sa
```

</details>
