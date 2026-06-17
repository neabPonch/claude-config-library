---
name: kotsutsumi__zylix
source: https://github.com/kotsutsumi/zylix/blob/7ca0965d7f1010f5d97bf5cf4f4bc143caadb557/CLAUDE.md
repo: kotsutsumi/zylix
kind: claude-md
stars: 55
last_pushed: 2026-03-15T09:52:33Z
license: apache-2.0
score: 9
domains: [systems-programming, cross-platform]
tags: [build-system, verification-checklist, api-versioning, zig]
curated: 2026-06-14
curated_by: config-scout
---

# kotsutsumi/zylix — claude-md

**Why it's worth keeping:** It includes vital version-specific API patterns (Zig 0.15 changes) to prevent hallucinated syntax and provides exact CLI flags for platform-specific target validation.

**Summary:** Defines strict cross-platform build requirements and verification steps for a multi-target Zig project.

**Source credibility:** The source is an active repository with recent commits, indicating a real-world development environment.

**Recency:** Highly current; specifically addresses the latest breaking changes in Zig's API.

**Source:** [kotsutsumi/zylix/CLAUDE.md](https://github.com/kotsutsumi/zylix/blob/7ca0965d7f1010f5d97bf5cf4f4bc143caadb557/CLAUDE.md) · 55★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Zylix Project - Claude Code Instructions

## Project Overview

Zylix is a cross-platform application runtime built with Zig core and native platform shells (iOS, Android, Web/WASM, Desktop).

## Project Structure

```
zylix/
├── core/                    # Zig core library
│   ├── src/
│   │   ├── main.zig        # Entry point, module exports
│   │   ├── state.zig       # State management
│   │   ├── events.zig      # Event system
│   │   ├── abi.zig         # C ABI exports for FFI
│   │   ├── ai/             # AI module (whisper, etc.)
│   │   └── animation/      # Animation module
│   │       ├── animation.zig    # Module exports
│   │       ├── timeline.zig     # Timeline and keyframe animation
│   │       ├── state_machine.zig # Animation state machine
│   │       ├── lottie.zig       # Lottie format support
│   │       └── live2d.zig       # Live2D format support
│   └── build.zig           # Zig build configuration
├── shells/
│   ├── ios/                # iOS Swift shell
│   ├── android/            # Android Kotlin shell
│   └── web/                # Web/WASM shell
└── site/                   # Documentation site
```

## Quality Verification Requirements

**IMPORTANT**: The
```

</details>
