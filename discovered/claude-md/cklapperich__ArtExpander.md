---
name: cklapperich__ArtExpander
source: https://github.com/cklapperich/ArtExpander/blob/76858798f6115a0358a4f0b8052ebe42edb33deb/CLAUDE.md
repo: cklapperich/ArtExpander
kind: claude-md
stars: 0
last_pushed: 2026-06-06T16:44:15Z
license: unknown
score: 8
domains: [.net, game-modding, unity]
tags: [bepinex, harmony, csharp]
curated: 2026-06-16
curated_by: config-scout
---

# cklapperich/ArtExpander — claude-md

**Why it's worth keeping:** The file excels at explaining 'hidden' logic flows—such as how code is injected via patches rather than standard inheritance—and provides critical domain-specific enum values to prevent hallucinations.

**Summary:** Provides a clear structural map of a Unity mod, detailing how Harmony patches and the art cache system interact with the game engine.

**Source credibility:** Low profile/individual project based on star count and description.

**Recency:** Current; targets modern .NET Standard and specific Unity versions used in current modding environments.

**Source:** [cklapperich/ArtExpander/CLAUDE.md](https://github.com/cklapperich/ArtExpander/blob/76858798f6115a0358a4f0b8052ebe42edb33deb/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

ArtExpander is a BepInEx mod for "Card Shop Simulator" that extends the game's artwork system. It allows custom artwork for different card border types (Base, FirstEdition, Silver, Gold, EX, FullArt) and expansion types, with special support for Destiny cards and Ghost expansions.

## Build Commands

**Build the project:**
```bash
dotnet build
```

**Build and package for distribution:**
```bash
./build.bat
```

The build.bat script:
1. Builds the project using `dotnet build`
2. Copies the DLL to `BepInEx/plugins/ArtExpander/`
3. Creates `ArtExpander.zip` containing the mod files

## Architecture

### Core Components

**Plugin.cs** - Main entry point that:
- Initializes the art cache from either `cardart/` or plugin root directory
- Applies Harmony patches for game integration
- Manages the plugin lifecycle

**ArtCache.cs** - Central artwork management system:
- Caches resolved file paths for (MonsterType, BorderType, ExpansionType) combinations
- Handles fallback logic for missing artwork
- Special handling for Ghost expansion (white/black varia
```

</details>
