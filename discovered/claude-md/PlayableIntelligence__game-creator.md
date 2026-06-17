---
name: PlayableIntelligence__game-creator
source: https://github.com/PlayableIntelligence/game-creator/blob/4e64b83b5fe400b34ad3a484d9b4a6090b26d512/CLAUDE.md
repo: PlayableIntelligence/game-creator
kind: claude-md
stars: 188
last_pushed: 2026-05-25T18:02:30Z
license: unknown
score: 9
domains: [game-dev, agents-ai, web-frontend]
tags: [agent-hooks, architectural-patterns, automation]
curated: 2026-06-15
curated_by: config-scout
---

# PlayableIntelligence/game-creator — claude-md

**Why it's worth keeping:** It defines ingenious 'agent hooks' like `render_game_to_text()` to allow LLMs to observe internal state without visual interpretation, and enforces singleton patterns to maintain consistency across multi-session tasks.

**Summary:** A sophisticated framework for AI-driven game development that utilizes a skill-based architecture and strict design patterns.

**Source credibility:** The repository has solid social proof with 188 stars and recent maintenance activity.

**Recency:** Highly relevant; it incorporates advanced agentic workflows using Playwright and structured state observation current for today's AI coding tools.

**Source:** [PlayableIntelligence/game-creator/CLAUDE.md](https://github.com/PlayableIntelligence/game-creator/blob/4e64b83b5fe400b34ad3a484d9b4a6090b26d512/CLAUDE.md) · 188★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## Project Overview

This is **game-creator**, the game studio for the agent internet. It provides skills and agents for scaffolding, designing, deploying, and monetizing 2D (Phaser 3) and 3D (Three.js) browser games. QA (build, runtime, visual review, autofix) runs at every step. Monetize with [Play.fun](https://play.fun) (OpenGameProtocol). Works with **40+ AI coding agents** (via `npx skills add`). Share your play.fun URL on [Moltbook](https://www.moltbook.com/).

## Repository Structure

```
.claude-plugin/
  plugin.json              # Plugin manifest (name, version, author)
  marketplace.json         # Marketplace metadata (owner: OpusGameLabs)
settings.json              # Default settings (activates game-creator agent)
skills/
  phaser/SKILL.md          # 2D game patterns (Phaser 3, scene-based, multi-file)
  threejs-game/SKILL.md    # 3D game patterns (Three.js, event-driven)
  threejs-perf/SKILL.md    # Three.js performance patterns with measured evidence (instancing static + moving)
  game-assets/SKILL.md     # Pixel art sprites (code-only, no external files)
  game-designer/SKILL.md   # Visual polish (gradients, particles, juice, transitions)
  game-audio/SKI
```

</details>
