---
name: OPENSPHERE-Inc__branch-output
source: https://github.com/OPENSPHERE-Inc/branch-output/blob/23401b7720caa3f176609556e21e511e0b909166/CLAUDE.md
repo: OPENSPHERE-Inc/branch-output
kind: claude-md
stars: 186
last_pushed: 2026-05-18T03:10:24Z
license: gpl-2.0
score: 9
domains: [c++, graphics, video-processing, desktop-apps]
tags: [cmake, cpp, architecture, build-system]
curated: 2026-06-15
curated_by: config-scout
---

# OPENSPHERE-Inc/branch-output — claude-md

**Why it's worth keeping:** The use of a detailed 'Repository Layout' with functional summaries and an 'Architecture & Key Concepts' table gives an LLM essential design context for complex C++ logic.

**Summary:** Provides a comprehensive structural and architectural map of the project, including granular toolchain requirements and functional file descriptions.

**Source credibility:** High; 186 stars and recent maintenance suggest a stable, real-world tool used by others.

**Recency:** Highly current; last pushed one month ago.

**Source:** [OPENSPHERE-Inc/branch-output/CLAUDE.md](https://github.com/OPENSPHERE-Inc/branch-output/blob/23401b7720caa3f176609556e21e511e0b909166/CLAUDE.md) · 186★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — Branch Output Plugin for OBS Studio

## Project Overview

**Branch Output** is an OBS Studio plugin (shared library / module) that adds an effect filter allowing
individual sources or scenes to stream and/or record independently from the main OBS output.
It is developed and maintained by **OPENSPHERE Inc.** under the GPLv2+ license.

- Repository language: **C++ 17** with **Qt 6** for UI
- Build system: **CMake** (≥ 3.16)
- Based on the official [obs-plugintemplate](https://github.com/obsproject/obs-plugintemplate)
- Target OBS Studio version: **≥ 30.1.0** (Qt6, x64 / ARM64 / Apple Silicon)

---

## Repository Layout

```
branch-output/
├── CMakeLists.txt          # Top-level CMake project definition
├── CMakePresets.json        # CMake presets (windows-x64, macos, linux-x86_64, CI variants)
├── buildspec.json           # Build specification (name, version, dependencies, UUIDs)
├── build.ps1                # Local Windows build script (RelWithDebInfo)
├── .clang-format            # C++ code style (clang-format ≥ 16)
├── .cmake-format.json       # CMake code style
├── .github/
│   ├── actions/             # Reusable format-check actions
│   └── workflows/           # C
```

</details>
