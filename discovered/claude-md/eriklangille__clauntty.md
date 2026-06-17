---
name: eriklangille__clauntty
source: https://github.com/eriklangille/clauntty/blob/775b683585c8b236b6a1113918cfa7c218768872/CLAUDE.md
repo: eriklangille/clauntty
kind: claude-md
stars: 400
last_pushed: 2026-02-13T18:44:32Z
license: unknown
score: 9
domains: [ios, systems-programming, mobile-dev]
tags: [swift, terminal, debugging-guide, build-automation]
curated: 2026-06-15
curated_by: config-scout
---

# eriklangille/clauntty — claude-md

**Why it's worth keeping:** The explicit breakdown of log levels/enablement and the detailed command groupings (e.g., sim.sh) provide a roadmap for an AI to debug itself. The inclusion of specific C API signatures allows an agent to understand and manipulate foreign language bindings without external searching.

**Summary:** A highly structured technical guide covering architecture, specialized build workflows, and tiered logging systems.

**Source credibility:** High; 400 stars and active development indicate a respected tool in the iOS/Terminal space.

**Recency:** Highly current (last pushed 4 months ago).

**Source:** [eriklangille/clauntty/CLAUDE.md](https://github.com/eriklangille/clauntty/blob/775b683585c8b236b6a1113918cfa7c218768872/CLAUDE.md) · 400★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Clauntty - iOS SSH Terminal with Ghostty

iOS SSH terminal using **libghostty** for GPU-accelerated rendering + **SwiftNIO SSH** for connections.

## Architecture

```
┌─────────────────────────────────────────────────────────────┐
│  SwiftUI Views              Direct I/O          SwiftNIO SSH │
│  ┌──────────────┐         ┌───────────┐      ┌────────────┐  │
│  │ Terminal UI  │ ──────► │ SSH Data  │ ───► │ SSH Channel│  │
│  │ + Keyboard   │ ◄────── │ Flow      │ ◄─── │ (remote)   │  │
│  └──────────────┘         └───────────┘      └────────────┘  │
│         │                                          │         │
│         ▼                                          ▼         │
│  GhosttyKit.xcframework                     Remote Server    │
│  (Metal rendering)                                           │
└─────────────────────────────────────────────────────────────┘
```

**Data Flow**:
- **SSH → Terminal**: `SSHChannelHandler.channelRead()` → `ghostty_surface_write_pty_output()` → rendered
- **Keyboard → SSH**: `insertText()` → `SSHConnection.sendData()` → SSH channel

## Repository Layout

```
~/Projects/clauntty/
├── clauntty/          # iOS app (this repo)
├── ghostty/
```

</details>
