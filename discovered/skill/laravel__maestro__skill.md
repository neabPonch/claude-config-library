---
name: laravel__maestro__skill
source: https://github.com/laravel/maestro/blob/2b8c595264ab57baebf4dbcf30e2bd879b0d7ca7/.agents/skills/maestro/SKILL.md
repo: laravel/maestro
kind: skill
stars: 66
last_pushed: 2026-06-15T10:46:46Z
license: unknown
score: 9
domains: [monorepo, devops, cli-tools, web-development]
tags: [orchestration, laravel, build-system, monorepo]
curated: 2026-06-15
curated_by: config-scout
---

# laravel/maestro — skill

**Why it's worth keeping:** It provides structured command tables with flag explanations and explains the logical folder hierarchy which is crucial for understanding how changes propagate. It also preemptively solves dependency issues by detailing necessary setup steps like `composer setup` before running CI checks.

**Summary:** A high-density skill file for a complex monorepo orchestrator that manages multiple starter kit variants through an inheritance-based layering system.

**Source credibility:** High; part of the official Laravel ecosystem with very recent activity.

**Recency:** Current; reflects modern development workflows including Bun, Vite-era tools, and specific framework linting needs.

**Source:** [laravel/maestro/.agents/skills/maestro/SKILL.md](https://github.com/laravel/maestro/blob/2b8c595264ab57baebf4dbcf30e2bd879b0d7ca7/.agents/skills/maestro/SKILL.md) · 66★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: maestro
description: >
  Maestro monorepo orchestrator for the official Laravel starter kits. Use this skill when making
  changes to any starter kit source files, building kits, running tests, or working with the kit
  inheritance hierarchy, placeholder system, teams feature, or any development workflow in this repo.
---

# Maestro Skill

## What is Maestro

Maestro is the monorepo orchestrator for the official [Laravel starter kits](https://laravel.com/starter-kits). All starter kit source files live here and get built out to individual repositories. Changes are made in this repo, and Maestro automatically creates PRs for the affected starter kit repos after merge.

## Project Structure

```
maestro/
├── kits/              # Source files for all starter kits (inheritance-based layering)
├── orchestrator/      # Laravel app that builds and watches starter kits
├── build/             # Generated starter kit (git-ignored) — make changes here during dev
├── browser_tests/     # Cross-kit browser tests for CI
└── .github/           # GitHub workflows
```

## Commands

All commands below run from the `orchestrator/` directory unless noted otherwise.

| Command
```

</details>
