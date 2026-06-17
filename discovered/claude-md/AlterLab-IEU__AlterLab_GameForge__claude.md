---
name: AlterLab-IEU__AlterLab_GameForge__claude
source: https://github.com/AlterLab-IEU/AlterLab_GameForge/blob/5f5148d61986b32299070e87fcd4a1ab3718eacf/starters/godot/CLAUDE.md
repo: AlterLab-IEU/AlterLab_GameForge
kind: claude-md
stars: 14
last_pushed: 2026-03-30T13:32:11Z
license: mit
score: 9
domains: [game-development, godot]
tags: [gdscript, godot-4, game-engine]
curated: 2026-06-16
curated_by: config-scout
---

# AlterLab-IEU/AlterLab_GameForge — claude-md

**Why it's worth keeping:** The 'Code Review Criteria' and 'Anti-Patterns' sections provide actionable checklists that transform the AI from a code generator into a specialized QA engineer. It also provides ready-to-use CLI commands for testing and exporting.

**Summary:** A highly prescriptive configuration for Godot 4.x that enforces strict GDScript typing, architectural patterns, and scene composition principles.

**Source credibility:** Good; part of a specialized indie game dev toolset with recent maintenance (3 months ago).

**Recency:** 

**Source:** [AlterLab-IEU/AlterLab_GameForge/starters/godot/CLAUDE.md](https://github.com/AlterLab-IEU/AlterLab_GameForge/blob/5f5148d61986b32299070e87fcd4a1ab3718eacf/starters/godot/CLAUDE.md) · 14★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Godot 4.x Engine Configuration

This section configures Claude Code for a Godot 4.x project. Append to your project's CLAUDE.md or use standalone.

## Engine Details

- **Engine**: Godot 4.6+
- **Primary Language**: GDScript (statically typed)
- **Engine Specialist**: `/game-godot-specialist`

When asking engine-specific questions, use `/game-godot-specialist`. For architecture questions that are engine-agnostic, use `/game-technical-director`.

## Project Structure

```
project.godot
scenes/               -- Scene files (.tscn)
  entities/           -- Player, enemies, NPCs
  levels/             -- Level/world scenes
  ui/                 -- UI scenes (menus, HUD, dialogs)
scripts/              -- GDScript files (.gd)
  autoloads/          -- Singleton autoload scripts
  components/         -- Reusable node components
  resources/          -- Custom Resource class definitions
  state_machines/     -- State machine implementations
  systems/            -- Core game systems (combat, inventory, etc.)
resources/            -- Resource files (.tres)
  data/               -- Gameplay data resources (stats, loot tables)
  themes/             -- UI themes
  materials/          -- Shader
```

</details>
