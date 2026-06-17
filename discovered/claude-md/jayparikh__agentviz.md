---
name: jayparikh__agentviz
source: https://github.com/jayparikh/agentviz/blob/099a7db12aef3da915d69ba62a68ab8a7f99be98/CLAUDE.md
repo: jayparikh/agentviz
kind: claude-md
stars: 88
last_pushed: 2026-06-14T10:45:51Z
license: mit
score: 9
domains: [web-frontend, ai-agent-tooling]
tags: [architecture-map, system-design]
curated: 2026-06-14
curated_by: config-scout
---

# jayparikh/agentviz — claude-md

**Why it's worth keeping:** The 'File -> Responsibility' mapping is a masterclass in providing context; it prevents the LLM from searching through files to find logic. Including 'Key data types' provides immediate schema awareness for state management.

**Summary:** A high-density architectural blueprint that maps specific files to their functional responsibilities and core data schemas.

**Source credibility:** High-quality specialized tool with recent activity and clear technical depth.

**Recency:** Very current; mentions Vite 6 and modern Claude Code integration.

**Source:** [jayparikh/agentviz/CLAUDE.md](https://github.com/jayparikh/agentviz/blob/099a7db12aef3da915d69ba62a68ab8a7f99be98/CLAUDE.md) · 88★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# AGENTVIZ

Session replay visualizer for AI agent workflows. Renders Claude Code, Codex, VS Code Copilot Chat, Copilot CLI, Copilot prompt exports, and ATIF / Harbor session logs as interactive timelines, with auto-detection of file format.

## Stack
- React 18 + Vite 6
- No CSS framework, all inline styles
- Font: JetBrains Mono (loaded from Google Fonts in index.html)
- Mixed JS/TS: components and hooks are plain JSX, parsers and data libs are TypeScript

## Architecture
```
src/
  App.jsx              # Default v2 mount + Classic UI fallback, theme wiring, session entry routing
  AppV2.jsx            # Default workflow shell: Find, Review, Investigate, Analyze, Compare, Improve
  main.jsx             # React entry point
  contexts/
    SessionProvider.jsx  # Shared session loading, discovery, compare, live, export, and derived state
    PlaybackContext.jsx  # Playback, search, track filtering, and derived state provider
  hooks/
    usePlayback.js     # Playback state: time, playing, speed, seek, playPause
    useSearch.js       # Debounced search with matchSet/matchedEntries
    useKeyboardShortcuts.js # Centralized keyboard handler (ref-based, stable listener)
    useQA.js
```

</details>
