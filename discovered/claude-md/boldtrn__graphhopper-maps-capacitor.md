---
name: boldtrn__graphhopper-maps-capacitor
source: https://github.com/boldtrn/graphhopper-maps-capacitor/blob/1d5a5fa05a4f47075c585d48719e9afbea8adc8d/CLAUDE.md
repo: boldtrn/graphhopper-maps-capacitor
kind: claude-md
stars: 32
last_pushed: 2026-05-22T16:28:42Z
license: apache-2.0
score: 9
domains: [mobile-app, android, gis]
tags: [capacitor, maplibre, kotlin]
curated: 2026-06-15
curated_by: config-scout
---

# boldtrn/graphhopper-maps-capacitor — claude-md

**Why it's worth keeping:** Includes critical 'anti-pattern' warnings regarding legacy Mapbox naming, explicit bridge flow diagrams, and highly detailed dependency/version tables that prevent hallucination in niche SDKs.

**Summary:** Provides deep technical context for a hybrid Capacitor-Android app with custom native navigation bridges.

**Source credibility:** High-quality technical documentation from a specialized open-source project.

**Recency:** Extremely current; updated within the last month.

**Source:** [boldtrn/graphhopper-maps-capacitor/CLAUDE.md](https://github.com/boldtrn/graphhopper-maps-capacitor/blob/1d5a5fa05a4f47075c585d48719e9afbea8adc8d/CLAUDE.md) · 32★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## Project Overview

Capacitor-based Android app wrapping **GraphHopper Maps** (React/OpenLayers web app) with a native **turn-by-turn navigation** screen built on MapLibre GL and the MapLibre Navigation SDK.

## Architecture

```
src/app.js                          -- Capacitor bridge: wires native APIs (TTS, clipboard, file, navigation)
                                       into window globals, then loads graphhopper-maps bundle
graphhopper-maps/                   -- git submodule (graphhopper/graphhopper-maps), React/OpenLayers web app
capacitor-maplibre-navigation/      -- Capacitor plugin: TypeScript definitions + Android Kotlin implementation
android/                            -- Main Android app shell (Capacitor host)
```

### Flow: Web -> Native Navigation

1. `graphhopper-maps` UI calls `window.ghNativeNavigation.start(url, body, onClose, miles)`
2. `src/app.js` bridges this to `MapLibreNavigation.startNavigation(...)` (Capacitor plugin call)
3. `MapLibreNavigationPlugin.kt` receives the call, launches `NavigationActivity`
4. On close, broadcast -> plugin -> JS `navigationClosed` event -> `onClose` callback

## capacitor-maplibre-navigation Plugin

### TypeS
```

</details>
