---
name: mxyhi__ok-skills__skill
source: https://github.com/mxyhi/ok-skills/blob/47e20bd789f593f68b5862464debc3d1bf9fa5bb/shader-dev/SKILL.md
repo: mxyhi/ok-skills
kind: skill
stars: 426
last_pushed: 2026-06-15T02:34:28Z
license: apache-2.0
score: 9
domains: [graphics, webgl, creative-coding]
tags: [glsl, shaders, ray-marching, procedural-generation]
curated: 2026-06-15
curated_by: config-scout
---

# mxyhi/ok-skills — skill

**Why it's worth keeping:** The Technique Routing Table is an elite pattern for managing domain-specific complexity; it provides the agent with a clear taxonomy of how to combine mathematical primitives into high-level effects.

**Summary:** A specialized knowledge orchestration system that maps complex graphic requests to specific GLSL implementation techniques. It uses a hierarchical routing table to ensure depth and technical accuracy in shader generation.

**Source credibility:** High; backed by significant GitHub community interest and recent activity.

**Recency:** Current; follows modern agentic skill patterns designed for LLM orchestration.

**Source:** [mxyhi/ok-skills/shader-dev/SKILL.md](https://github.com/mxyhi/ok-skills/blob/47e20bd789f593f68b5862464debc3d1bf9fa5bb/shader-dev/SKILL.md) · 426★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: shader-dev
description: Comprehensive GLSL shader techniques for creating stunning visual effects — ray marching, SDF modeling, fluid simulation, particle systems, procedural generation, lighting, post-processing, and more.
license: MIT
metadata:
  version: "1.0"
  category: graphics
---

# Shader Craft

A unified skill covering 36 GLSL shader techniques (ShaderToy-compatible) for real-time visual effects.

## Invocation

```
/shader-dev <request>
```

`$ARGUMENTS` contains the user's request (e.g. "create a raymarched SDF scene with soft shadows").

## Skill Structure

```
shader-dev/
├── SKILL.md                      # Core skill (this file)
├── techniques/                   # Implementation guides (read per routing table)
│   ├── ray-marching.md           # Sphere tracing with SDF
│   ├── sdf-3d.md                 # 3D signed distance functions
│   ├── lighting-model.md         # PBR, Phong, toon shading
│   ├── procedural-noise.md       # Perlin, Simplex, FBM
│   └── ...                       # 34 more technique files
└── reference/                    # Detailed guides (read as needed)
    ├── ray-marching.md           # Math derivations & advanced patterns
    ├── sd
```

</details>
