---
name: mecharoy__OrbitDefense__game-skill
source: https://github.com/mecharoy/OrbitDefense/blob/9dbe75f439476fdf2b3490881673e59d82f1baf0/GAME.skill.md
repo: mecharoy/OrbitDefense
kind: skill
stars: 0
last_pushed: 2025-11-21T20:01:29Z
license: unknown
score: 7
domains: [web-game-dev, frontend-performance]
tags: [ecs, canvas-optimization, deterministic-logic]
curated: 2026-06-16
curated_by: config-scout
---

# mecharoy/OrbitDefense — skill

**Why it's worth keeping:** Provides specific implementation strategies like fixed time step accumulators, object pooling to avoid GC pauses, and multi-layered canvas rendering.

**Summary:** A high-performance technical specification for building deterministic browser games using ECS and canvas optimization.

**Source credibility:** Low visibility (0 stars); likely an individual developer's internal technical documentation.

**Recency:** Current; reflects modern web game development and deployment standards.

**Source:** [mecharoy/OrbitDefense/GAME.skill.md](https://github.com/mecharoy/OrbitDefense/blob/9dbe75f439476fdf2b3490881673e59d82f1baf0/GAME.skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
Development & Deployment Best Practices1. Code Quality & StructureECS Pattern (Entity-Component-System)Instead of deep OOP inheritance (e.g., class Guard extends Enemy extends Actor), use composition.Entities: Just IDs (e.g., Entity_1).Components: Data containers (e.g., Position, Velocity, Sprite, InputRecorder).Systems: Logic processors (e.g., MovementSystem updates all entities with Position and Velocity).Why? This makes managing the "Ghosts" significantly easier. The Ghost is just an entity with a InputReplay component instead of a InputListener component.Deterministic StateFor the time-loop replay to work, your game logic must be deterministic.Fixed Time Step: Do not rely on variable deltaTime for physics simulation. Use a fixed time step accumulator (e.g., 1/60th of a second) to ensure the ghost moves exactly the same distance as the player did, regardless of frame rate fluctuations.Avoid Randomness: Do not use Math.random() for anything affecting gameplay during the level. If you must, use a seeded random number generator so the "random" guard patrol is identical across loops.Object PoolingBrowser games suffer from Garbage Collection (GC) pauses.Never create new objects insid
```

</details>
