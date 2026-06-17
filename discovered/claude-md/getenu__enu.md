---
name: getenu__enu
source: https://github.com/getenu/enu/blob/3d79834511285ff6a5f6c151660d3c187d12d3e5/CLAUDE.md
repo: getenu/enu
kind: claude-md
stars: 478
last_pushed: 2026-06-11T20:30:06Z
license: mit
score: 9
domains: [game-engine, systems-programming]
tags: [nim, godot, build-system, 3d-graphics]
curated: 2026-06-15
curated_by: config-scout
---

# getenu/enu — claude-md

**Why it's worth keeping:** Contains high-value instructions on avoiding manual edits to generated files, specific exception handling patterns, and strict casing rules. Includes meta-instructions to prevent AI attribution in commits.

**Summary:** Provides comprehensive guidance for a specialized Nim/Godot engine, covering complex build processes and dual type systems.

**Source credibility:** Highly reputable project with significant stars and recent activity.

**Recency:** Modern; includes relevant guidelines for agentic workflow (commit hygiene/attribution).

**Source:** [getenu/enu/CLAUDE.md](https://github.com/getenu/enu/blob/3d79834511285ff6a5f6c151660d3c187d12d3e5/CLAUDE.md) · 478★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Enu is a 3D sandbox environment for creating and exploring voxel worlds using a Logo-inspired programming API. It's built with Nim and the Godot game engine (v3.5), enabling users to program interactive 3D environments using Nim scripts that run in the Nim VM.

## Build Commands

### Setup
- `atlas install && atlas rep` - Install dependencies (first-time setup)
- `nim prereqs` - Build Godot, download fonts, generate API bindings and stdlib

### Dependency Management (Atlas)

- `atlas.lock` pins exact dependency versions
- `atlas pin <package>` - Update lock file for a specific package after changing its version in deps/
- `atlas install` - Install dependencies from lock file
- `atlas rep` - Regenerate nim.cfg paths from lock file
- When changing dependencies in enu.nimble, run `atlas install && atlas pin` to update the lock file

### Generated Artifacts

**Never manually edit files that are meant to be produced by tools** (lock files, sentinel files, zip archives, etc.), even if you know how to make the required changes. We need to verify our too
```

</details>
