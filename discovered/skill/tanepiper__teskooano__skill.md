---
name: tanepiper__teskooano__skill
source: https://github.com/tanepiper/teskooano/blob/71c2beb70f0880bdf7adf97c0cd7f19c5a015e75/.agent/skills/webgl/SKILL.md
repo: tanepiper/teskooano
kind: skill
stars: 26
last_pushed: 2026-03-23T09:33:15Z
license: other
score: 8
domains: [web-frontend, graphics-programming, security]
tags: [webgl, shaders, gpu, typescript, threejs]
curated: 2026-06-15
curated_by: config-scout
---

# tanepiper/teskooano — skill

**Why it's worth keeping:** Provides highly transferable patterns like memory-tracked resource management (WebGLResourceManager), context loss handling, and type-safe uniform validation utilities.

**Summary:** A high-quality technical skill file for low-level WebGL development, focusing on GPU safety, resource management, and performance.

**Source credibility:** Niche repository with high code density suggesting specialized expertise rather than generic boilerplate.

**Recency:** Current; utilizes WebGL 2.0 standards and modern TypeScript/Vue-style composable patterns.

**Source:** [tanepiper/teskooano/.agent/skills/webgl/SKILL.md](https://github.com/tanepiper/teskooano/blob/71c2beb70f0880bdf7adf97c0cd7f19c5a015e75/.agent/skills/webgl/SKILL.md) · 26★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: webgl
description: WebGL shaders and effects for JARVIS 3D HUD
model: sonnet
risk_level: MEDIUM
version: 1.0.0
---

# WebGL Development Skill

> **File Organization**: This skill uses split structure. See `references/` for advanced patterns and security examples.

## 1. Overview

This skill provides WebGL expertise for creating custom shaders and visual effects in the JARVIS AI Assistant HUD. It focuses on GPU-accelerated rendering with security considerations.

**Risk Level**: MEDIUM - Direct GPU access, potential for resource exhaustion, driver vulnerabilities

**Primary Use Cases**:

- Custom shaders for holographic effects
- Post-processing effects (bloom, glitch)
- Particle systems with compute shaders
- Real-time data visualization

## 2. Core Responsibilities

### 2.1 Fundamental Principles

1. **TDD First**: Write tests before implementation - test shaders, contexts, and resources
2. **Performance Aware**: Optimize GPU usage - batch draws, reuse buffers, compress textures
3. **GPU Safety**: Implement timeout mechanisms and resource limits
4. **Shader Validation**: Validate all shader inputs before compilation
5. **Context Management**: Handle context loss graceful
```

</details>
