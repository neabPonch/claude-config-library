---
name: TheGabmeister__games-unreal__claude
source: https://github.com/TheGabmeister/games-unreal/blob/a2f89110254ecacb43370069c525b32919678af9/CrashBandicoot/CLAUDE.md
repo: TheGabmeister/games-unreal
kind: claude-md
stars: 1
last_pushed: 2026-05-22T03:14:47Z
license: unknown
score: 9
domains: [game-development, unreal-engine, automation]
tags: [ue5, build-system, procedural-generation, workflow-automation]
curated: 2026-06-15
curated_by: config-scout
---

# TheGabmeister/games-unreal — claude-md

**Why it's worth keeping:** It includes specific troubleshooting (Live Coding conflicts), precise build commands with path handling, and detailed instructions for external toolchain scripts (Blender/Python) that prevent AI-driven workflow breaks.

**Summary:** Provides an exhaustive operational manual for managing a complex Unreal Engine project via CLI and custom automation tools.

**Source credibility:** High technical density for a small-scale repo; indicates a highly structured development pipeline.

**Recency:** Very current, specifically addressing modern automation patterns like MCP bridges and complex engine build requirements.

**Source:** [TheGabmeister/games-unreal/CrashBandicoot/CLAUDE.md](https://github.com/TheGabmeister/games-unreal/blob/a2f89110254ecacb43370069c525b32919678af9/CrashBandicoot/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**CB** (CrashBandicoot) is a Crash Bandicoot-style 3D platformer built with Unreal Engine 5.7 (C++/Blueprints). The `.uproject` file is `CB.uproject`. The UE5 engine lives at `C:\Program Files\Epic Games\UE_5.7`.

## Related Documents

- **SPEC.md** — complete gameplay spec for the Crash Bandicoot 1996 recreation (mechanics, rules, values, enemy behaviors, boss fights, level list, etc.). Follows the 1996 original, NOT the N. Sane Trilogy.
- **PHASES.md** — ordered implementation phases with deliverables and playtest criteria
- **PLAN_00.md** — Phase 0 rename plan (completed)
- **PLAN_01.md** — Phase 1 core player plan (movement, spin, camera, input, animation)
- **PLAN_02.md** — Phase 2 crates & collectibles plan (crates, pickups, Aku Aku, lives, damage)
- **PLAN_03.md** — Phase 3 enemies plan (10 archetype classes, chain-kill, projectiles, hazards, turtle platform)

## Build Commands

Always use Bash (not PowerShell) for build commands — PowerShell permission patterns have escaping issues.

```bash
# Build editor (Development)
"C:\Program Files\
```

</details>
