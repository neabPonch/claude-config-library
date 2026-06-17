---
name: TheGoodDoktor__8BitAnalysers
source: https://github.com/TheGoodDoktor/8BitAnalysers/blob/b004aceb5aeaa79195c82b4c75cdd12523c693c7/CLAUDE.md
repo: TheGoodDoktor/8BitAnalysers
kind: claude-md
stars: 130
last_pushed: 2026-06-14T21:49:06Z
license: mit
score: 9
domains: [game-development, systems-programming, cli-tools]
tags: [cmake, cpp, architecture, coding-standards]
curated: 2026-06-15
curated_by: config-scout
---

# TheGoodDoktor/8BitAnalysers — claude-md

**Why it's worth keeping:** It provides essential 'First run' setup instructions to prevent environment failures and contains highly specific naming convention rules (prefixes) that are perfect for maintaining code consistency via AI.

**Summary:** A high-quality technical guide for a complex multi-project C++ build system that includes critical runtime configuration steps.

**Source credibility:** High; a well-starred project with active maintenance and clear structure.

**Recency:** Current; explicitly mentions Claude Code and includes modern MCP server integration details.

**Source:** [TheGoodDoktor/8BitAnalysers/CLAUDE.md](https://github.com/TheGoodDoktor/8BitAnalysers/blob/b004aceb5aeaa79195c82b4c75cdd12523c693c7/CLAUDE.md) · 130★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

8-Bit Analysers is a suite of GUI tools for analysing and annotating games on 8-bit systems (ZX Spectrum, C64, CPC, BBC Micro, Arcade Z80, Tube Elite). Each analyser is a separate CMake project sharing a large common library. This repo is on the `ArcadeZ80` branch, which adds arcade Z80 game analysis support.

## Build Commands

Each analyser lives under `Source/<AnalyserName>/`. Build steps are identical across all of them:

```bash
cd Source/ArcadeZ80   # or ZXSpectrum, C64, CPC, BBC, TubeElite
mkdir build && cd build
cmake ..
# Linux/macOS:
make
# macOS Xcode project:
cmake -G Xcode ..
# Windows: opens Visual Studio solution generated in build/
```

Binaries are output to `build/bin/`. The VS debugger working directory is set to `../../Data/ArcadeZ80` in the CMake project, so on Windows run the executable from `Data/ArcadeZ80/`.

**First run:** copy `Data/<AnalyserName>/imgui.ini` to your working directory. Edit the generated `globalconfig.json` to set `WorkspaceRoot`, `SnapshotFolder`, and `PokesFolder` paths.

**Clone with submodules:**
```b
```

</details>
