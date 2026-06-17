---
name: feldoh__TotalControl
source: https://github.com/feldoh/TotalControl/blob/1d7508bc92d31de4e4887a1610fdecc4416d21a7/CLAUDE.md
repo: feldoh/TotalControl
kind: claude-md
stars: 2
last_pushed: 2026-06-06T12:02:06Z
license: mit
score: 9
domains: [game-development, c#, modding]
tags: [architecture, performance-optimization, data-persistence, compatibility]
curated: 2026-06-16
curated_by: config-scout
---

# feldoh/TotalControl — claude-md

**Why it's worth keeping:** The 'CRITICAL' sections define non-negotiable guardrails for performance, data persistence (DefRef pattern), and backward compatibility. It successfully bridges high-level architectural intent with low-level coding requirements like brace usage and translation patterns.

**Summary:** A highly detailed technical manual that covers build systems, architecture hierarchy, and strict domain-specific development rules.

**Source credibility:** High; demonstrates expert-level mastery of the RimWorld/Harmony modding ecosystem and professional software lifecycle management.

**Recency:** Current; specifically targets the latest version (1.6) and modern .NET build workflows.

**Source:** [feldoh/TotalControl/CLAUDE.md](https://github.com/feldoh/TotalControl/blob/1d7508bc92d31de4e4887a1610fdecc4416d21a7/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**Total Control** (assembly name: `FactionLoadout`) is a RimWorld mod that enables deep customization of faction pawns — appearance, equipment, genes, hediffs, and more. It uses Harmony patches to intercept pawn generation and apply user-defined edits.

## Build Commands

```bash
# Release build (formats code, creates zip, copies to Steam if configured)
dotnet build -c Release

# The solution file is also available
dotnet build FactionLoadout.sln
```

Output DLLs go to `{version}/Assemblies/`. Release builds produce `FactionLoadout.zip` at the repo root.

### Environment Variables (optional)
- `RIMWORLD_PATH` — RimWorld install directory (fallback: `../../../../` relative to Source)
- `STEAM_MODS_PATH` or `RIMWORLD_STEAM_MODS_PATH` — Steam workshop mods directory (release copies mod here)

If local RimWorld DLLs aren't found, the build falls back to the `Krafs.Rimworld.Ref` NuGet package.

## Code Structure

### Version Layout
Three parallel source trees for RimWorld 1.4, 1.5, and 1.6:
```
1.4/Source/  1.5/Source/  1.6/Source/   # C# source (1.6
```

</details>
