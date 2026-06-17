---
name: expo__expo__claude
source: https://github.com/expo/expo/blob/f0700472ff7dd007969df860b24116d24977c130/packages/@expo/log-box/CLAUDE.md
repo: expo/expo
kind: claude-md
stars: 50079
last_pushed: 2026-06-15T06:46:21Z
license: mit
score: 9
domains: [web-frontend, mobile-development]
tags: [architecture, technical-spec]
curated: 2026-06-15
curated_by: config-scout
---

# expo/expo — claude-md

**Why it's worth keeping:** The 'Key Files for Common Tasks' table is a premier pattern for AI navigation; ASCII diagrams provide essential mental models of complex state transitions.

**Summary:** A high-density technical blueprint detailing the LogBox error system's architecture, data flows, and platform-specific implementations.

**Source credibility:** Extremely high; comes from the industry-standard Expo repository.

**Recency:** Current, featuring very recent migration history and active maintenance.

**Source:** [expo/expo/packages/@expo/log-box/CLAUDE.md](https://github.com/expo/expo/blob/f0700472ff7dd007969df860b24116d24977c130/packages/@expo/log-box/CLAUDE.md) · 50079★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# @expo/log-box

A universal error overlay for Expo apps that displays runtime errors, warnings, and build errors with symbolicated stack traces.

## Package Structure

```
src/
├── Data/                    # State management and data parsing
│   ├── LogBoxData.tsx       # Central state store (observer pattern)
│   ├── LogBoxLog.ts         # Log object + React context
│   ├── parseLogBoxLog.ts    # Error parsing and categorization
│   └── Types.ts             # TypeScript definitions
├── overlay/                 # Full-screen error inspector
│   ├── Overlay.tsx          # Main inspector component
│   ├── Header.tsx           # Top bar with controls
│   ├── StackTraceList.tsx   # Animated stack trace display
│   ├── CodeFrame.tsx        # Code snippet with syntax highlighting
│   ├── Message.tsx          # Error message rendering
│   ├── AnsiHighlight.tsx    # ANSI terminal color parsing
│   └── *.module.css         # CSS modules for each component
├── toast/                   # Minimal error notification
│   ├── ErrorToast.tsx       # Bottom-left toast
│   └── ErrorToast.module.css
├── utils/                   # Shared utilities
│   ├── renderInShadowRoot.ts    # Shadow DOM isolati
```

</details>
