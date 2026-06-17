---
name: CXWorld__CapFrameX
source: https://github.com/CXWorld/CapFrameX/blob/383bc029adba29bdbedf96b922713dec48acf76b/CLAUDE.md
repo: CXWorld/CapFrameX
kind: claude-md
stars: 1223
last_pushed: 2026-06-14T10:13:57Z
license: other
score: 9
domains: [desktop-app, windows, c++, .net]
tags: [msbuild, mvvm, native-interop, performance-analysis]
curated: 2026-06-16
curated_by: config-scout
---

# CXWorld/CapFrameX — claude-md

**Why it's worth keeping:** Explicitly breaks down the multi-project architecture into logical layers (UI, Core, Data, Native) which is vital for large repositories; includes precise MSBuild commands that bypass generic 'build' ambiguity.

**Summary:** Detailed documentation for a complex Windows desktop application involving mixed C#/.NET and native C++ code. It provides specific build instructions for main apps, native components, and installers.

**Source credibility:** High: widely used performance tool with significant star count and recent activity.

**Recency:** 

**Source:** [CXWorld/CapFrameX/CLAUDE.md](https://github.com/CXWorld/CapFrameX/blob/383bc029adba29bdbedf96b922713dec48acf76b/CLAUDE.md) · 1223★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

CapFrameX is a Windows desktop application for frametime capture and analysis, built on Intel's PresentMon. It provides an overlay via Rivatuner Statistics Server (RTSS) and is used for gaming performance benchmarking.

## Build Commands

### Prerequisites
- Visual Studio 2022
- WiX Toolset v3.14.1 with VS 2022 Extension
- C++ MFC build tools

### Build the Main Application
```bash
nuget restore CapFrameX.sln
msbuild source\CapFrameX\CapFrameX.csproj /p:Configuration=Release /p:Platform=x64 /p:VisualStudioVersion=17.0
```

### Build Native C++ Components (required for full functionality)
```bash
msbuild source\CapFrameX.Hwinfo\CapFrameX.Hwinfo.vcxproj /p:SolutionDir=%CD%\ /p:Configuration=Release /p:Platform=x64 /p:VisualStudioVersion=17.0
msbuild source\CapFrameX.IGCL\CapFrameX.IGCL.vcxproj /p:SolutionDir=%CD%\ /p:Configuration=Release /p:Platform=x64 /p:VisualStudioVersion=17.0
msbuild source\CapFrameX.ADLX\CapFrameX.ADLX.vcxproj /p:SolutionDir=%CD%\ /p:Configuration=Release /p:Platform=x64 /p:VisualStudioVersion=17.0
```

### Build Installer
`
```

</details>
