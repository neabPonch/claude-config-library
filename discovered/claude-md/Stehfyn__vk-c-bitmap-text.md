---
name: Stehfyn__vk-c-bitmap-text
source: https://github.com/Stehfyn/vk-c-bitmap-text/blob/29cb150d402c38a4fc7b8e422ab8621293dcb057/CLAUDE.md
repo: Stehfyn/vk-c-bitmap-text
kind: claude-md
stars: 0
last_pushed: 2026-03-28T23:37:10Z
license: mit
score: 8
domains: [graphics, c-programming, vulkan]
tags: [low-level, build-automation, shader-workflow]
curated: 2026-06-16
curated_by: config-scout
---

# Stehfyn/vk-c-bitmap-text — claude-md

**Why it's worth keeping:** The instruction for handling shaders (source + embedded SPIR-V + updated build script) is a perfect template for managing assets in low-level languages. It also enforces a high-quality decision-making process via the trade-off proposal rule.

**Summary:** Provides strict constraints for maintaining a minimal C99 Vulkan project, focusing on build integrity and specific shader integration workflows.

**Source credibility:** A specialized, niche example repository; value is derived from its specific technical constraints rather than popularity.

**Recency:** Very recent (3 months ago), highly relevant to current development workflows.

**Source:** [Stehfyn/vk-c-bitmap-text/CLAUDE.md](https://github.com/Stehfyn/vk-c-bitmap-text/blob/29cb150d402c38a4fc7b8e422ab8621293dcb057/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# vk-c-bitmap-text

A minimal example of bitmap text rendering in Vulkan 1.2 with Vulkan best practices and written in C99

## Overview

- Purpose: Exemplify bitmap text rendering in Vulkan with straightforward shaders and pipeline(s).
- Tech: C99, GLSL 4.5+, SPIR-V, VulkanSDK, MSVC14, Visual Studio 2022, WindowsSDK
- Priorities: Correctness, best-practices, and clear uncomplicated code.

## Repository map (adjust as needed)

- `build.bat` — Build vk-c-bitmap-text.exe
- `vk-c-bitmap-text.sln` — Visual Studio 2022 Solution
- `vk-c-bitmap-text/` — All vk-c-bitmap-text.sln's projects
- `res/fonts/` - Monospace example font(s)

## Conventions

- Formatting: Allman braces
- Styling: Vulkan API styling and naming conventions, Win32

## Runbook 

- Build: `build.bat`

## Guardrails for Claude

- Keep focused on producing a minimal example of bitmap text rendering in Vulkan 1.2 with Vulkan best practices and written in C99
- When asked to implement, ask any questions you have that you're wondedring about
- Do not introduce breaking changes. `build.bat` must succeed, and `vk-c-bitmap-text.exe` **must return 0**
- If adding shaders, add the original shader code file, embed the compiled SPIR-
```

</details>
