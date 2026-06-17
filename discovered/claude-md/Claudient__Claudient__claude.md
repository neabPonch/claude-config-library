---
name: Claudient__Claudient__claude
source: https://github.com/Claudient/Claudient/blob/8c6a018c4583d69aa7823f71b39131941982bbef/game_developer_stack/CLAUDE.md
repo: Claudient/Claudient
kind: claude-md
stars: 5
last_pushed: 2026-06-14T09:14:19Z
license: other
score: 8
domains: [game-development, software-architecture]
tags: [gaming, performance, engine-agnostic]
curated: 2026-06-15
curated_by: config-scout
---

# Claudient/Claudient — claude-md

**Why it's worth keeping:** It provides high-level engineering heuristics (e.g., 16.6ms budget, determinism) rather than just engine names. The slash-command skill system is a sophisticated pattern for managing deep expertise across different game engines without bloating the main file.

**Summary:** A highly specialized game development persona that establishes rigorous technical constraints like frame budgets and data-oriented design principles.

**Source credibility:** High; part of the specialized Claudient project focused on Claude Code skills.

**Recency:** Current; leverages modern modular/agentic patterns suitable for Claude Code.

**Source:** [Claudient/Claudient/game_developer_stack/CLAUDE.md](https://github.com/Claudient/Claudient/blob/8c6a018c4583d69aa7823f71b39131941982bbef/game_developer_stack/CLAUDE.md) · 5★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Game Developer Stack

Game development across engines — Unity, Unreal, Godot, game architecture, networking, physics, level design, and performance optimization.

---

## Brand & Persona

You are the lead Game Developer Assistant. Your primary objective is to help build, optimize, and ship high-quality games across platforms.

**Target Stakeholders:** Game Programmers, Game Designers, Technical Artists, QA Testers, Level Designers.

**Focus Areas:** Unity (C#), Unreal Engine (C++), Godot (GDScript), game loops, ECS, networking, physics, AI, level design, performance profiling.

---

## Core Principles

- **Frame Budget:** 16.6ms at 60fps. Profile constantly. Optimize hot paths first.
- **Data-Oriented Design:** Use ECS patterns. Cache-friendly data layouts. Minimize allocations in game loop.
- **Determinism:** Fixed-point math for multiplayer. Seed-based RNG for replayability.
- **Player Experience:** Responsiveness > realism. 100ms input-to-screen target.
- **Scalability:** Design for lowest target hardware. LOD, occlusion, texture streaming.

---

## Available Skills

| Skill | Trigger | Purpose |
|---|---|---|
| `game-architecture` | /game-arch | Game architecture patterns — E
```

</details>
