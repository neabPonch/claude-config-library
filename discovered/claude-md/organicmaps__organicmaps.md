---
name: organicmaps__organicmaps
source: https://github.com/organicmaps/organicmaps/blob/307fad9178406cf7ebbcd9b54095d9cdfb875a58/CLAUDE.md
repo: organicmaps/organicmaps
kind: claude-md
stars: 14326
last_pushed: 2026-06-15T02:38:35Z
license: other
score: 9
domains: [mobile-dev, systems-programming, cross-platform]
tags: [c++, architecture, multi-platform, build-system]
curated: 2026-06-15
curated_by: config-scout
---

# organicmaps/organicmaps — claude-md

**Why it's worth keeping:** It provides concrete code snippets for include conventions and testing macros, ensuring the agent follows project-specific patterns rather than generic ones; it also enforces architectural constraints like layer hierarchy.

**Summary:** A comprehensive technical manual covering layered architecture, multi-platform build processes, and strict C++/Swift coding standards.

**Source credibility:** High-quality open-source project (Organic Maps) with significant community traction and active maintenance.

**Recency:** Current, referencing modern C++23 standards and recent build tools.

**Source:** [organicmaps/organicmaps/CLAUDE.md](https://github.com/organicmaps/organicmaps/blob/307fad9178406cf7ebbcd9b54095d9cdfb875a58/CLAUDE.md) · 14326★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Agent Instructions for Organic Maps

Organic Maps (OM) is an open-source, privacy-focused offline maps & GPS app built on OpenStreetMap data.
OM works on iOS, Android, and desktop (Windows, macOS, Linux using Qt 6).
The codebase is mostly C++23 with platform-specific code in Swift 5, Objective-C/C++, Java 17 and tools in bash and Python 3.10+

## Architecture overview

Libraries in `libs/` are strictly layered -- no circular or upward dependencies allowed:

1. **Foundation:** `base` (logging, assertions, caches), `coding` (serialization, I/O), `geometry` (points, rects, mercator)
2. **Platform:** `platform` (file paths, HTTP, location -- OS-abstracted via `*_ios.mm`, `*_android.cpp`, `*_qt.cpp`)
3. **Data:** `indexer` (map features, classification), `kml`, `transit`, `routing_common`, `editor`
4. **Domain:** `search`, `routing`, `storage` (map downloads), `traffic`
5. **Rendering:** `drape` (OpenGL/Vulkan/Metal abstraction), `drape_frontend` (scene management), `shaders`
6. **Application:** `map` (Framework class -- aggregates all subsystems)
7. **UI:** in the project's root: `qt/` (desktop), `iphone/` (iOS), `android/` (Android), `dev_sandbox/` (graphics dev tool)

Key namespace
```

</details>
