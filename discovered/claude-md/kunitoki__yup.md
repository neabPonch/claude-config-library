---
name: kunitoki__yup
source: https://github.com/kunitoki/yup/blob/12b796252c71d49128dea37ff5e7f2b441849b42/CLAUDE.md
repo: kunitoki/yup
kind: claude-md
stars: 148
last_pushed: 2026-06-13T11:30:29Z
license: other
score: 9
domains: [cpp, graphics, audio-engine]
tags: [cpp-standard, architecture-templates, module-management, testing-patterns]
curated: 2026-06-15
curated_by: config-scout
---

# kunitoki/yup — claude-md

**Why it's worth keeping:** The use of literal code blocks for file headers and module metadata ensures perfect consistency; the 'AI Decision Making' section provides actionable architectural heuristics rather than generic platitudes.

**Summary:** Provides highly prescriptive structural blueprints for a C++ graphics/audio library, including exact file headers, module declarations, and class templates.

**Source credibility:** High-quality source from a specialized graphics/audio framework with recent activity.

**Recency:** Current; aligns well with modern C++20 workflows and Claude Code's agentic capabilities.

**Source:** [kunitoki/yup/CLAUDE.md](https://github.com/kunitoki/yup/blob/12b796252c71d49128dea37ff5e7f2b441849b42/CLAUDE.md) · 148★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# AI Assistant Guidelines for YUP Project

This document provides directive guidelines for AI assistants working on the YUP project. Use these rules when generating, reviewing, or suggesting code changes.

## Project Context
- **Project Type:** C++ graphics/audio library
- **License:** ISC License
- **Copyright:** `Copyright (c) 2026 - kunitoki@gmail.com`
- **Based On:** Fork of JUCE7 ISC Modules
- **Build System:** CMake
- **Testing Framework:** Google Test
- **Primary Dependencies:** Rive, OpenGL/Metal/D3D
- **C++ Standard**: >= C++20

## Code Generation Rules

**NEVER EVER run bash commands to configure, compile or test the implementation, acknowledge that we should test and we'll run and report any issue.**

## AI Decision Making Rules

### Always:
1. **Rely on the C++20 language and standard library** so use it (unless the feature is not supported in all YUP's platforms)
2. **Check existing patterns** in similar modules first
3. **Use YUP conventions** for similar functionality
4. **Use YUP infrastructure** instead of reinventing the wheel
5. **If the same functionality can be provided with less code and complexity** prefer less code
6. **Always prefer reusing code than creati
```

</details>
