---
name: forketyfork__architect
source: https://github.com/forketyfork/architect/blob/f85e3e3670c6654f856e7831be871b4d4f9fc074/CLAUDE.md
repo: forketyfork/architect
kind: claude-md
stars: 40
last_pushed: 2026-06-14T08:15:56Z
license: mit
score: 9
domains: [cli-tools, systems-programming, graphics]
tags: [zig, sdl3, low-level]
curated: 2026-06-16
curated_by: config-scout
---

# forketyfork/architect — claude-md

**Why it's worth keeping:** The 'Gotchas' section prevents subtle type-inference bugs, and the 'Observability' section clearly defines how to handle the gap between terminal execution and visual rendering.

**Summary:** A highly specialized technical manual that provides deep guardrails for a low-level Zig and SDL3 codebase.

**Source credibility:** Strong; comes from an active, specialized systems programming project.

**Recency:** Very current, specifically referencing recent Zig 0.15 API changes.

**Source:** [forketyfork/architect/CLAUDE.md](https://github.com/forketyfork/architect/blob/f85e3e3670c6654f856e7831be871b4d4f9fc074/CLAUDE.md) · 40★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md (symlinked as AGENTS.md)

[Canonical file: `CLAUDE.md`. Keep `AGENTS.md` as a symlink to `CLAUDE.md`.]

## Project

**Name:** Architect
**Description:** A terminal multiplexer and AI-assisted coding environment built on SDL3 and Zig. Architect lets developers run multiple terminal sessions in a tiled layout, annotate diffs, and integrate Claude agents directly into their workflow.
**Stack:** Zig 0.15, SDL3, ghostty-vt (terminal emulation), Nix dev shell, `just` task runner
**Status:** Active development

## Build & Run

```bash
# Worktree bootstrap (run in a fresh worktree)
just setup   # pre-caches the ghostty-vt tarball; skip if already cached

# Environment activation
nix develop  # or: direnv allow
#
# Minimal host prerequisites:
# - Nix with flakes enabled (or direnv + nix-direnv)
# - macOS (primary platform; Linux support is partial)

# Build
zig build

# Run
zig build run

# Test
zig build test

# Type check
N/A  # Zig build covers type checking

# Lint
just lint

# Format check
zig fmt --check src/
```

## Infrastructure

- **Source code hosting:** GitHub — URL: `https://github.com/forketyfork/architect` — CLI: `gh` — Skill: `managing-github`
- **Issue tracker:*
```

</details>
