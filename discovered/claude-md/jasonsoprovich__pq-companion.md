---
name: jasonsoprovich__pq-companion
source: https://github.com/jasonsoprovich/pq-companion/blob/8a8453ea22402fca2dc3283a36471a2f44e84cda/claude.md
repo: jasonsoprovich/pq-companion
kind: claude-md
stars: 2
last_pushed: 2026-06-13T19:22:51Z
license: unknown
score: 9
domains: [desktop-app, go-backend, react-frontend, game-development]
tags: [architecture-heavy, domain-knowledge, multi-process]
curated: 2026-06-14
curated_by: config-scout
---

# jasonsoprovich/pq-companion — claude-md

**Why it's worth keeping:** It utilizes negative constraints (e.g., 'do not use Prettier'), clarifies the responsibility split between processes, and provides critical domain-specific data mapping essential for accurate code generation.

**Summary:** A highly detailed guide for a complex Go/Electron/React application that includes specific architectural rules and niche business logic.

**Source credibility:** High-quality specialized tool with very recent maintenance activity.

**Recency:** Very current; uses modern tech stacks including Go 1.22 and Tailwind v4.

**Source:** [jasonsoprovich/pq-companion/claude.md](https://github.com/jasonsoprovich/pq-companion/blob/8a8453ea22402fca2dc3283a36471a2f44e84cda/claude.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# PQ Companion — Claude Code Project Instructions

## Project Overview
PQ Companion is a desktop companion app for the EverQuest emulated server
"Project Quarm." The app is feature-complete and currently in a
fine-tuning, bug-fixing, and maintenance phase — most ongoing work is
polish, regressions, and incorporating periodic Project Quarm database
updates.

Capabilities (see `FEATURES.md` for the full implementation log):
- Database explorer (items, spells, NPCs, zones) with global Cmd/Ctrl+K search
- Combat log parser, DPS/HPS meter, and combat history with per-combatant breakdowns
- Spell timer engine with separate buff and detrimental overlays
- NPC info overlay (level, class, HP, resists, special abilities) keyed off the active target
- Spell checklist cross-referenced against the Zeal spellbook export
- Inventory tracker and key tracker (raid key components) across all characters
- Character info pages (stats, AAs, spell modifiers)
- Config backup manager for EQ `.ini` files
- GINA-style custom trigger system with regex patterns, on-screen alerts, audio alerts, and importable trigger packs
- Auto-updating Windows installer

## Architecture
- **Go backend** (`backend/`): API se
```

</details>
