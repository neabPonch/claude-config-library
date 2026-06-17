---
name: Viclaww__madeinblaccApp
source: https://github.com/Viclaww/madeinblaccApp/blob/14d8ea2b829cb40e8e8b3a0cd5d89c27f5e4d300/claude.md
repo: Viclaww/madeinblaccApp
kind: claude-md
stars: 0
last_pushed: 2026-06-11T13:01:50Z
license: unknown
score: 8
domains: [mobile-development, react-native]
tags: [ignite, expo, typescript, style-conventions]
curated: 2026-06-14
curated_by: config-scout
---

# Viclaww/madeinblaccApp — claude-md

**Why it's worth keeping:** The inclusion of explicit code patterns (like the $themed style factory) and a 'Definition of Done' prevents architectural drift. It also enforces tool-chain consistency by mandating the use of the Ignite CLI.

**Summary:** Provides highly specific structural, stylistic, and workflow constraints for an Ignite/React Native project.

**Source credibility:** Low star count, but reflects high-quality professional architecture standards.

**Recency:** Highly current with modern React Native/Expo development patterns.

**Source:** [Viclaww/madeinblaccApp/claude.md](https://github.com/Viclaww/madeinblaccApp/blob/14d8ea2b829cb40e8e8b3a0cd5d89c27f5e4d300/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Copilot Instructions for This Ignite App

This repository is an Ignite + Expo + TypeScript React Native app.
Generate code that matches Ignite conventions and existing project patterns.

## Instruction Priority

Apply these rules in this order:

1. Follow existing code in the repository first.
2. Follow Ignite architecture and patterns.
3. Apply these instructions when no stronger local pattern exists.

## Core Stack

- Expo
- React Native
- TypeScript
- Ignite
- React Navigation
- MobX-State-Tree (MST)
- Reactotron
- Jest
- React Native Testing Library
- Detox

## Architecture and File Placement

Use Ignite structure only:

- app/screens
- app/components
- app/models
- app/services
- app/utils
- app/theme

Do not introduce new architecture layers or arbitrary top-level folders unless requested.

Generator CLI

- Use the Ignite CLI to add new screens and components so generated files follow project conventions and templates (for example: `ignite generate screen MyScreen` or `ignite generate component MyComponent`). Prefer the CLI-generated files over manual file creation to keep app structure consistent.

## State Management (MST)

- Use MST for global and shared domain state.
-
```

</details>
