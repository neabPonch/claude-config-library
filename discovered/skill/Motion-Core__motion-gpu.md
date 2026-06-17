---
name: Motion-Core__motion-gpu
source: https://github.com/Motion-Core/motion-gpu/blob/3ba7c72edb74ef416122ef39f30da22c4ba482d5/SKILL.md
repo: Motion-Core/motion-gpu
kind: skill
stars: 175
last_pushed: 2026-06-15T01:09:34Z
license: mit
score: 9
domains: [web-frontend, graphics, webgpu]
tags: [webgpu, wgsl, svelte, react, vue]
curated: 2026-06-15
curated_by: config-scout
---

# Motion-Core/motion-gpu — skill

**Why it's worth keeping:** Uses 'Hard Contracts' to prevent hallucinated WGSL/WebGPU errors and includes a detailed source of truth table for specific package entrypoints.

**Summary:** A highly specialized skill file that provides deep context for the MotionGPU WebGPU framework across multiple frontend adapters.

**Source credibility:** High; derived from an active, specialized WebGPU framework with recent maintenance.

**Recency:** Current; aligns with modern component-based architecture and active repository status.

**Source:** [Motion-Core/motion-gpu/SKILL.md](https://github.com/Motion-Core/motion-gpu/blob/3ba7c72edb74ef416122ef39f30da22c4ba482d5/SKILL.md) · 175★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: motion-gpu-adapters-wgsl
description: Build and edit MotionGPU code across framework-agnostic core and Svelte/React/Vue adapters. Use when implementing or refactoring FragCanvas-based components, defineMaterial shaders, useFrame runtime logic, textures/useTexture workflows, render passes/targets, compute shaders/storage buffers, render-mode scheduling, or MotionGPU error handling and diagnostics.
---

# MotionGPU Core + Adapters Skill

Use this skill to produce production-grade MotionGPU code across:
- framework-agnostic core (`@motion-core/motion-gpu`, `@motion-core/motion-gpu/core`),
- Svelte adapter (`@motion-core/motion-gpu/svelte`),
- React adapter (`@motion-core/motion-gpu/react`),
- Vue adapter (`@motion-core/motion-gpu/vue`).

Treat Svelte, React, and Vue as first-class adapters. Do not assume Svelte-only APIs.

## Source of Truth

Treat public package entrypoints as authoritative:

| Entrypoint | Layer | What it exposes |
| --- | --- | --- |
| `@motion-core/motion-gpu` | Core | Framework-agnostic runtime primitives (`defineMaterial`, `resolveMaterial`, scheduler/runtime builders, passes, texture loader, error normalization) |
| `@motion-core/motion-gpu/advanced`
```

</details>
