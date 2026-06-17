---
name: meodai__skill.color-expert
source: https://github.com/meodai/skill.color-expert/blob/14a8deee7b3b010893a26391dd51a7c1648e5c75/CLAUDE.md
repo: meodai/skill.color-expert
kind: claude-md
stars: 489
last_pushed: 2026-06-10T10:56:29Z
license: other
score: 7
domains: [agents-ai, knowledge-management]
tags: [agent-skills, structured-documentation, knowledge-base]
curated: 2026-06-15
curated_by: config-scout
---

# meodai/skill.color-expert — claude-md

**Why it's worth keeping:** Demonstrates a specific technique to prevent context bloat: keeping the core skill file concise while offloading density to a organized directory tree; provides rules for maintaining trigger accuracy.

**Summary:** Defines a structured architecture for an agent skill, separating high-level 'trigger' logic from deep technical reference files.

**Source credibility:** High star count (489) and active maintenance suggest it is a leading example of this specialized pattern.

**Recency:** Current; specifically optimized for modern agentic workflows like Claude Code.

**Source:** [meodai/skill.color-expert/CLAUDE.md](https://github.com/meodai/skill.color-expert/blob/14a8deee7b3b010893a26391dd51a7c1648e5c75/CLAUDE.md) · 489★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance when working with code in this repository.

## Project Overview

This is an **agent skill** (compatible with Claude Code, Codex, Cursor, Copilot, OpenCode, and others via [agentskills.io](https://agentskills.io)). It contains a `SKILL.md` file that serves as a color expertise knowledge base, automatically loaded when the agent handles color-related tasks (naming, theory, spaces, accessibility, perception).

## Architecture

- `SKILL.md` — The skill definition with YAML frontmatter (`name`, `description`) and structured color knowledge. Loaded when color work is detected.
- `references/INDEX.md` — Master lookup table for 140+ deep reference files.
- `references/historical/` — Pre-digital color science (Ostwald, Helmholtz, ISCC-NBS, etc.)
- `references/contemporary/` — Modern color science (OKLAB, Briggs, CSA webinars, etc.)
- `references/techniques/` — Tools, libraries, methods (Spectral.js, Culori, APCA, palette generation, etc.)

## No Build/Test/Lint

There are no commands to run. This project is purely declarative content consumed by agent skill systems.

## Editing Guidelines

- Keep SKILL.md frontmatter `description` field accurate — it
```

</details>
