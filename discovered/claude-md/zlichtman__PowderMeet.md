---
name: zlichtman__PowderMeet
source: https://github.com/zlichtman/PowderMeet/blob/d3a7613673a654bd0089799d9059faa06408cfde/CLAUDE.md
repo: zlichtman/PowderMeet
kind: claude-md
stars: 1
last_pushed: 2026-05-24T17:30:24Z
license: other
score: 9
domains: [ios, mobile-app]
tags: [architecture-mapping, state-management, structural-documentation]
curated: 2026-06-16
curated_by: config-scout
---

# zlichtman/PowderMeet — claude-md

**Why it's worth keeping:** The 'App shell' section explains data-flow and lifecycle ownership (e.s., how the coordinator manages services), while the directory map includes functional constraints and public API requirements for specific modules.

**Summary:** This file provides a high-density architectural blueprint that maps out state management flow and component responsibilities. It bridges the gap between raw file structure and application logic.

**Source credibility:** A niche, specialized project with high-quality technical documentation.

**Recency:** Current; explicitly mentions Swift 6 and Xcode 16.

**Source:** [zlichtman/PowderMeet/CLAUDE.md](https://github.com/zlichtman/PowderMeet/blob/d3a7613673a654bd0089799d9059faa06408cfde/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# PowderMeet — Claude orientation

Ski-meetup iOS app that finds the optimal meeting point between two skiers on a
mountain. "FATMAP merged with Find My" — Mapbox satellite-streets base, stylized
overlays, realtime presence, pathfinding across a directed trail/lift graph.

For setup (secrets, Mapbox token, Supabase schema), see `README.md`.

## Stack

- **iOS:** Swift 6 + SwiftUI, Xcode 16 Synchronized Folders. New `.swift` files
  auto-register; no `.pbxproj` edits needed.
- **Map:** MapboxMaps SDK (satellite-streets-v12 style).
- **Backend:** Supabase — auth, Postgres, Realtime (Broadcast + postgres_changes).
- **On-device cache:** SwiftData (`FriendLocationStore`, `LocationHistoryStore`).
- **Build:** Open `PowderMeet.xcodeproj` in Xcode. Target family is iPhone
  only (`TARGETED_DEVICE_FAMILY = "1"`). PowderMeet is a one-handed-on-a-
  chairlift, in-a-pocket-with-gloves app — iPad layout isn't a use case
  worth shipping. All four build configs (app + tests, Debug + Release)
  are pinned to iPhone.
- **SPM deps:** `MapboxMaps`, `Supabase`. SourceKit often can't resolve these
  in isolation — "No such module" / "Cannot find type" diagnostics are usually
  project-resolution nois
```

</details>
