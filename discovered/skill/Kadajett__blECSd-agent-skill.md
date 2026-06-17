---
name: Kadajett__blECSd-agent-skill
source: https://github.com/Kadajett/blECSd-agent-skill/blob/eb7df13aaa5d7815d0fbaf0544cf54f6cd29c435/Skill.md
repo: Kadajett/blECSd-agent-skill
kind: skill
stars: 0
last_pushed: 2026-02-10T09:31:27Z
license: mit
score: 7
domains: [cli-tools, typescript, game-development]
tags: [ecs, architecture, technical-spec]
curated: 2026-06-14
curated_by: config-scout
---

# Kadajett/blECSd-agent-skill — skill

**Why it's worth keeping:** It utilizes a high-density 'Guardrails' section to prevent anti-patterns and provides an explicit execution phase workflow (Input/Layout/Render) that is easily digestible by an agent.

**Summary:** A highly structured technical specification defining architectural constraints and lifecycle workflows for the blECSd TypeScript library.

**Source credibility:** Low-star personal repository, but the content shows professional-grade architectural depth.

**Recency:** Recent; last updated 4 months ago.

**Source:** [Kadajett/blECSd-agent-skill/Skill.md](https://github.com/Kadajett/blECSd-agent-skill/blob/eb7df13aaa5d7815d0fbaf0544cf54f6cd29c435/Skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: blecsd-codex-skill
description: Best practices and module map for blECSd (TypeScript terminal UI). Use when building, reviewing, or refactoring blECSd apps, widgets, systems, or ECS/game-loop code.
---

# blECSd Codex Skill

Use this skill to build, review, or refactor blECSd applications and libraries.

## Follow Core Principles

- Treat blECSd as a library, not a framework.
- Use functional style only: pure functions, plain data, no classes.
- Use ECS patterns: entities as IDs, components as SoA data, systems as pure transforms.
- Keep input responsive: INPUT phase runs first and drains events.

## Choose an API

- Use Game API for games and real-time apps.
- Use ECS API for full control and performance tuning.

## Apply the Recommended Workflow

1. Pick the API surface.
- Import from `blecsd` for typical apps.
- Import from `blecsd/terminal` for low-level terminal control.
- Import from `blecsd/components` and `blecsd/systems` for custom pipelines.

2. Create the world and screen.
- Call `createWorld` and `createScreenEntity` for ECS API.
- Call `createGame` for Game API.

3. Build UI with the right abstraction.
- Use widgets for rapid development.
- Use entity factori
```

</details>
