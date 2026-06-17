---
name: RandallLiuXin__GodotMaker__claude-tmpl
source: https://github.com/RandallLiuXin/GodotMaker/blob/e7b66f05913787baac0d02d89e963ab0f1529407/skills/core/project-scaffold/templates/claude.md.tmpl
repo: RandallLiuXin/GodotMaker
kind: claude-md
stars: 307
last_pushed: 2026-06-15T05:52:53Z
license: other
score: 9
domains: [game-development, ecs]
tags: [godot, gdscript, ecs]
curated: 2026-06-15
curated_by: config-scout
---

# RandallLiuXin/GodotMaker — claude-md

**Why it's worth keeping:** Includes code snippets as few-shot pattern templates and provides highly specific CLI commands that allow Claude to self-correct via headless builds and test runs.

**Summary:** Defines a strict ECS architecture for Godot using the gecs framework and provides explicit commands for testing and build verification.

**Source credibility:** Strong; a specialized project with significant community interest (307 stars) and recent activity.

**Recency:** Very current; utilizes advanced Claude Code patterns like custom skill documentation.

**Source:** [RandallLiuXin/GodotMaker/skills/core/project-scaffold/templates/claude.md.tmpl](https://github.com/RandallLiuXin/GodotMaker/blob/e7b66f05913787baac0d02d89e963ab0f1529407/skills/core/project-scaffold/templates/claude.md.tmpl) · 307★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## Project: {{game_title}}

{{game_description}}

Built with Godot 4.x and the gecs ECS framework.

## Architecture

ECS-native: components are data, systems are logic, entities are component bags.

### Directory Layout

- `src/components/` — C_ prefix, extends Component, @export vars only
- `src/systems/` — PascalCase + System suffix, extends System
- `src/entities/` — extends Entity, define_components()
- `scenes/` — .tscn scene files; gameplay scene contains a World child
  node wired via `ECS.world = $World` in the main script's `_ready()`
  (autoloading World breaks gecs v7.1.0)
- `test/` — gdUnit4 tests (TDD: test first, then implement)

### ECS Rules

1. Components hold data only — no logic, no methods that modify other components
2. Systems query entities by component composition and run logic each frame
3. One system writes each data field per entity — no write conflicts
4. Entity destruction: add DestroyTag component, DestructionSystem handles cleanup at frame end
5. Physics callbacks: never modify node tree directly — only add components or use SetDeferred

### gecs Quick Reference

```gdscript
# Component — pure data
class_name C_Velocity extends Component
```

</details>
