---
name: SamWatson86__echo-chamber
source: https://github.com/SamWatson86/echo-chamber/blob/0be83b943f5849bf70cf22d2a2b571b571226d05/CLAUDE.md
repo: SamWatson86/echo-chamber
kind: claude-md
stars: 1
last_pushed: 2026-06-01T18:33:24Z
license: unknown
score: 9
domains: [rust, tauri, windows, devops]
tags: [autonomy, worktree-management, process-control]
curated: 2026-06-16
curated_by: config-scout
---

# SamWatson86/echo-chamber — claude-md

**Why it's worth keeping:** Includes specific shell commands for killing elevated processes and a precise manual protocol for syncing files from worktrees back to the main repo. The 'User Persona' section provides elite instructions on where the AI should act autonomously vs. when to guide.

**Summary:** Defines a high-agency workflow for an AI agent managing a complex local Rust/Tauri environment for a non-technical user. It bridges the gap between code changes and system-level deployment.

**Source credibility:** Specific, high-signal personal project with very recent activity.

**Recency:** Highly current; optimized for Claude Code's ability to execute terminal commands and manage local files.

**Source:** [SamWatson86/echo-chamber/CLAUDE.md](https://github.com/SamWatson86/echo-chamber/blob/0be83b943f5849bf70cf22d2a2b571b571226d05/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Echo Chamber - Project Context

## What Is This?
A self-hosted video conferencing app for Sam and friends ("The Fellowship of the Boatrace"). Uses LiveKit SFU for WebRTC media, Rust control plane, Tauri native Windows client, and web viewer. Built for 1080p@60fps with adaptive quality.

## Sam Is NOT A Developer
- Do NOT ask Sam to run commands, edit files, or debug
- Do NOT ask for confirmation before local operations — FULL AUTONOMY for local work
- Use `Start-Process -Verb RunAs` when elevated permissions needed (Sam clicks UAC prompt)
- Guide and explain, don't instruct

## NEVER Push to GitHub for Server Changes
- The server runs on Sam's local PC. Server changes deploy by rebuild + restart locally.
- GitHub pushes are ONLY for client releases (Tauri installer distributed to friends)
- Client releases use version tags: `git tag v0.X.Y && git push --tags` (triggers CI)
- CI is `workflow_dispatch` (manual) for builds, tag-triggered for releases
- **Ask Sam before ANY `git push` operation**

## Architecture
- **LiveKit SFU** (`core/sfu/`) — Native Windows binary, WebRTC media routing
- **Rust Control Plane** (`core/control/`) — HTTPS server (axum), room management, auth, API en
```

</details>
