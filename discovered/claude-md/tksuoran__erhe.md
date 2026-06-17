---
name: tksuoran__erhe
source: https://github.com/tksuoran/erhe/blob/ba5dccbffda662feb056f9ebc37d6a3b9a6fed19/CLAUDE.md
repo: tksuoran/erhe
kind: claude-md
stars: 878
last_pushed: 2026-06-14T19:16:01Z
license: other
score: 9
domains: [graphics, cpp, build-systems]
tags: [architecture-warnings, session-handoff, build-orchestration, maintenance-guidance]
curated: 2026-06-15
curated_by: config-scout
---

# tksuoran/erhe — claude-md

**Why it's worth keeping:** Includes 'rotten code' instructions to avoid wasted refactoring effort; features a unique `next_prompt.txt` pattern for multi-session state management; and provides highly specific initialization order warnings that prevent common C++ logic errors.

**Summary:** A high-quality guide that manages complex build processes across platforms and provides critical architectural warnings to prevent runtime crashes. It also implements a custom session handoff protocol for context continuity.

**Source credibility:** High-quality, well-maintained C++ graphics library with significant GitHub star count (878).

**Recency:** Very recent/current; includes modern developer environment references like VS 2026 and Claude Code specific workflows.

**Source:** [tksuoran/erhe/CLAUDE.md](https://github.com/tksuoran/erhe/blob/ba5dccbffda662feb056f9ebc37d6a3b9a6fed19/CLAUDE.md) · 878★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**erhe** is a C++ graphics library and editor for Vulkan, OpenGL and Metal (Vulkan is the default backend). It features a render graph system, full 3D scene graph, physics (Jolt), geometry manipulation (Catmull-Clark, Conway operators via Geogram), and an ImGui-based editor application.

## Session handoff: `next_prompt.txt`

When an untracked `next_prompt.txt` exists in the repo root, it is a handoff written by an older Claude Code session so that work can continue with fresh context: read it first and continue the work it describes. Once it has been read and the work is done, simply delete the file - do not update it or keep it around. Notes about the work done must already be in the commit messages for that work, so no information is lost by deleting it. (Writing a new `next_prompt.txt` is only warranted when handing off still-unfinished work to a future session.)

## `src/rendering_test/` is rotten

`src/rendering_test/` (the standalone `rendering_test` executable, its own duplicated shaders under `res/rendering_test/shaders/`, and its `cell_
```

</details>
