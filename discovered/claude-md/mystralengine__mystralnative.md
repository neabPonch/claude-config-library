---
name: mystralengine__mystralnative
source: https://github.com/mystralengine/mystralnative/blob/cea857ddb04cb05226aa630c3d9f674c4b3251d5/CLAUDE.md
repo: mystralengine/mystralnative
kind: claude-md
stars: 380
last_pushed: 2026-06-07T18:40:07Z
license: mit
score: 9
domains: [graphics-engine, native-development]
tags: [webgpu, build-system, negative-constraints]
curated: 2026-06-17
curated_by: config-scout
---

# mystralengine/mystralnative — claude-md

**Why it's worth keeping:** It uses 'Negative Constraints' to prevent common errors and provides high-fidelity build/test commands that are crucial for autonomous agents performing environment setup or maintenance.

**Summary:** Provides critical negative constraints to prevent using deprecated native loaders and gives detailed command-line workflows for building, testing, and releasing.

**Source credibility:** High; from an active, star-rated native WebGPU engine repository.

**Recency:** Current; reflects modern CI/CD and build practices.

**Source:** [mystralengine/mystralnative/CLAUDE.md](https://github.com/mystralengine/mystralnative/blob/cea857ddb04cb05226aa630c3d9f674c4b3251d5/CLAUDE.md) · 380★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# MystralNative - Claude Code Instructions

This document contains important instructions for AI assistants working on the MystralNative codebase.

## Critical Rules

### DO NOT Use Native GLTF/GLB Loaders

**NEVER** use or reference the C++ native GLTF/GLB loading code in this repository. The files exist but are deprecated and will cause compile errors if included:

- `src/gltf/gltf_loader.cpp` - DEPRECATED
- `src/utils/cgltf_impl.cpp` - DEPRECATED
- `include/mystral/gltf/gltf_loader.h` - DEPRECATED
- `third_party/cgltf/` - DEPRECATED

**Why?** MystralNative should use the **JavaScript GLBLoader/GLTFLoader** from the Mystral web engine (same code that runs in browsers). This ensures:

1. **Feature parity** with the web engine
2. **Consistent behavior** across platforms (web, desktop, mobile)
3. **Extension support** like Draco mesh compression (via WASM)
4. **Easier maintenance** - one codebase for all platforms

### How to Load GLTF/GLB Files

In your JavaScript/TypeScript code running on MystralNative, use:

```javascript
// For GLB files (binary GLTF)
import { loadGLBModel } from 'mystral';
const model = await loadGLBModel(device, './path/to/model.glb');

// For GLTF files (JSO
```

</details>
