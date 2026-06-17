---
name: LeithKetchell__UrhoVulkan
source: https://github.com/LeithKetchell/UrhoVulkan/blob/235566b6dcdf41fcdd68da76e44aa9e9df7ccfaf/CLAUDE.md
repo: LeithKetchell/UrhoVulkan
kind: claude-md
stars: 1
last_pushed: 2026-05-26T17:26:21Z
license: unknown
score: 9
domains: [agents-ai, cli-tools, concurrency]
tags: [orchestration, multi-agent, process-management]
curated: 2026-06-15
curated_by: config-scout
---

# LeithKetchell/UrhoVulkan — claude-md

**Why it's worth keeping:** Uses safe build wrappers with file-locking to prevent race conditions during multi-agent builds. Implements a trust/verification hierarchy to filter signal from noise in agent communications.

**Summary:** Defines orchestration protocols for multiple concurrent Claude Code instances communicating via IPC and a centralized WorkboardManager. It provides strict rules for process spawning, task state transitions, and hierarchy-based communication.

**Source credibility:** Low star count but the technical sophistication suggests high-level systems engineering for AI orchestration.

**Recency:** Current, based on recent pushes (1 month ago).

**Source:** [LeithKetchell/UrhoVulkan/CLAUDE.md](https://github.com/LeithKetchell/UrhoVulkan/blob/235566b6dcdf41fcdd68da76e44aa9e9df7ccfaf/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**Urho3D** is a free, lightweight, cross-platform 2D and 3D game engine implemented in C++, released under the MIT license. It supports multiple scripting languages (AngelScript, Lua) and multiple rendering backends (OpenGL, Direct3D 11).

- **Current Version**: 2.0.1
- **Build System**: CMake 3.15+
- **Supported Platforms**: Windows, Linux, macOS, iOS, tvOS, Android, Web (Emscripten), Raspberry Pi
- **Documentation**: https://urho3d.io/documentation
- **Contributing**: https://urho3d.io/documentation/HEAD/_contribution_checklist.html

## Session Startup Protocol

Claude Code instances in this project coordinate via IPC hooks and a WorkboardManager GUI. Every instance is a coder — there are no other roles.

On session start:

1. You are auto-registered on startup via the SessionStart hook — no manual action needed
2. Run `.claude/hooks/claude_ipc.sh assume auto` to grab the next free coder slot
3. Check in with Leith for your assignment
4. The Manager can reach you between prompts — react to incoming messages and keep listening

**PID files and i
```

</details>
