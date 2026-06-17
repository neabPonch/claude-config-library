---
name: rhemvi__omaclip
source: https://github.com/rhemvi/omaclip/blob/54fd601634f60d10dae5ba3eb078880fd55499ef/CLAUDE.md
repo: rhemvi/omaclip
kind: claude-md
stars: 13
last_pushed: 2026-04-17T18:16:29Z
license: mit
score: 9
domains: [desktop-app, security, systems-programming]
tags: [go, wails, networking, security]
curated: 2026-06-15
curated_by: config-scout
---

# rhemvi/omaclip — claude-md

**Why it's worth keeping:** Provides exact cryptographic and networking protocols (TLS/mDNS) rather than high-level summaries; enforces strict architectural boundaries and CSS constraints to prevent style drift.

**Summary:** A technical specification for a secure, cross-platform clipboard manager using Go and Vue.

**Source credibility:** High quality; demonstrates deep domain knowledge in systems programming and security protocols.

**Recency:** Extremely current for modern agentic workflows requiring high-precision technical instructions.

**Source:** [rhemvi/omaclip/CLAUDE.md](https://github.com/rhemvi/omaclip/blob/54fd601634f60d10dae5ba3eb078880fd55499ef/CLAUDE.md) · 13★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Omaclip — Project Instructions

## Overview

A Wails desktop clipboard manager that tracks clipboard history and syncs across multiple computers on the local network.

## Tech Stack

- **Backend**: Go (Wails v2)
- **Frontend**: Vue 3 + Vite + Pinia
- **CSS**: TailwindCSS only — no other CSS frameworks, no custom CSS classes outside of Tailwind utilities
- **Peer Discovery**: mDNS via `grandcat/zeroconf` (`_omaclip._tcp` service type)
- **Sync Transport**: HTTPS with TLS — a CA cert is derived from the passphrase and used to sign a leaf cert; peers validate against this CA (no `InsecureSkipVerify`)

## Features

1. **Clipboard history** — continuously poll/monitor the system clipboard and store a history of copied items (text and PNG images)
2. **History UI** — browse and re-copy from clipboard history
3. **Multi-machine sync** — peers discover each other via mDNS and pull each other's clipboard over HTTPS
4. **Omarchy theming** — automatically reads the active Omarchy color theme and applies it to the UI; colors update live when the theme changes
5. **Remote clipboard disable** — `--remote-clipboards-disable` flag skips networking entirely for single-machine use

## Clipboard His
```

</details>
