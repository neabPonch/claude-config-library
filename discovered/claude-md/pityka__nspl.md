---
name: pityka__nspl
source: https://github.com/pityka/nspl/blob/f58e76339bd0074ca15dcd00181775af26754114/CLAUDE.md
repo: pityka/nspl
kind: claude-md
stars: 101
last_pushed: 2026-05-16T14:47:52Z
license: other
score: 9
domains: [scientific-computing, data-visualization, scala]
tags: [architecture-first, build-automation, technical-deep-dive]
curated: 2026-06-15
curated_by: config-scout
---

# pityka/nspl — claude-md

**Why it's worth keeping:** The 'Architecture' section explains design patterns (Scene Graph) and complex logic flows (Event/Interaction models), which prevents an LLM from violating structural invariants. It also maps high-level concepts directly to specific source files for faster navigation.

**Summary:** This file provides comprehensive build instructions and a detailed architectural walkthrough of the project's scene graph and event systems.

**Source credibility:** High-quality specialized scientific library with notable community interest (101 stars).

**Recency:** Current; reflects recent development and modern Scala ecosystem standards.

**Source:** [pityka/nspl/CLAUDE.md](https://github.com/pityka/nspl/blob/f58e76339bd0074ca15dcd00181775af26754114/CLAUDE.md) · 101★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

nspl is a 2D scientific plotting library for Scala and Scala.js. It supports scatter, line, contour, raster, bar, box, histogram, and density plots with rendering backends for JVM (AWT/PDF/SVG/EPS) and browser (HTML5 Canvas/SVG).

## Build Commands

```bash
sbt -J-Xmx3000m +compile              # Compile all modules for both Scala versions
sbt saddle/test                        # Run Saddle integration tests (the main test suite)
sbt awt/test                           # Run AWT rendering tests
sbt versionPolicyCheck                 # Enforce binary compatibility (run by CI)
sbt scalafmtAll                        # Format all sources with Scalafmt
sbt docs/mdoc docs/unidoc             # Generate documentation
```

CI runs: `sbt -J-Xmx3000m +compile saddle/test versionPolicyCheck`

## Module Structure

- **core** / **coreJS** — Platform-agnostic plotting logic (scene graph, axes, data rendering, layouts). No external dependencies.
- **sharedJvm** / **sharedJs** — Shared utilities bridging core to platform-specific code.
- **awt** — JVM rendering vi
```

</details>
