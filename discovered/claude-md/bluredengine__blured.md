---
name: bluredengine__blured
source: https://github.com/bluredengine/blured/blob/751280b94cc7203d7f08f604699ef3c8b1f0b9d7/CLAUDE.md
repo: bluredengine/blured
kind: claude-md
stars: 12
last_pushed: 2026-03-27T08:20:14Z
license: other
score: 8
domains: [game-engine, systems-programming, cpp]
tags: [godot, debugging-workflow, coding-standards, engine-dev]
curated: 2026-06-16
curated_by: config-scout
---

# bluredengine/blured — claude-md

**Why it's worth keeping:** The 'Auto-iterate' debugging loop is a brilliant way to leverage agentic behavior, and the ASCII-only constraint prevents common C++ UI corruption errors.

**Summary:** Defines a specialized workflow for modifying a custom engine built on Godot and OpenCode. It includes high-precision rules for debugging loops and character encoding constraints.

**Source credibility:** Niche engine project; instructions appear written by an engineer managing a specific build process.

**Recency:** Very current (pushed 3 months ago).

**Source:** [bluredengine/blured/CLAUDE.md](https://github.com/bluredengine/blured/blob/751280b94cc7203d7f08f604699ef3c8b1f0b9d7/CLAUDE.md) · 12★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Blured Engine Development Rules

## Core Principle
You are free to modify **Godot Engine source code** (`godot/`) and **OpenCode source code** (`opencode/`) to fully integrate these two components. Always choose the best approach for building a new AI-powered game engine.

## Architecture
- **blured Engine** = Godot Engine + OpenCode AI
- Godot provides the game engine, editor, and runtime
- OpenCode provides AI orchestration, LLM integration, and natural language processing

## Guidelines

### When to Modify Engine Source
- Add native support for AI features directly in Godot when it improves performance or UX
- Modify OpenCode to add Godot-specific tools, routes, or behaviors
- Create deep integrations that wouldn't be possible with plugins alone

### When to Use Plugins/Extensions
- For features that don't require engine-level access
- For rapid prototyping before committing to engine changes
- For optional features that users may want to disable

### Build Commands
- **Full build**: `/build-blured`
- **Start engine**: `/start-blured`

### Key Paths
- Godot source: `godot/`
- OpenCode source: `opencode/`

### Terminology
- **AA** = AI Assistant (the built-in AI chat panel in t
```

</details>
