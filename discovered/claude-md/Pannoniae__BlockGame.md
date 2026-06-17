---
name: Pannoniae__BlockGame
source: https://github.com/Pannoniae/BlockGame/blob/d8d8ecbb092b4f9a2867848e8137036f31411205/CLAUDE.md
repo: Pannoniae/BlockGame
kind: claude-md
stars: 33
last_pushed: 2026-06-13T23:19:32Z
license: other
score: 8
domains: [game-engine, csharp, .net]
tags: [high-performance, architecture-heavy, low-level]
curated: 2026-06-15
curated_by: config-scout
---

# Pannoniae/BlockGame — claude-md

**Why it's worth keeping:** Effective use of specific build/run commands to manage terminal noise and explicit instructions on how to navigate the codebase (searching partial classes).

**Summary:** Defines a high-competence persona and provides deep architectural hierarchies for a custom C# game engine.

**Source credibility:** Active, niche project with moderate social proof via stars.

**Recency:** Highly current; leverages bleeding-edge .NET 10/C# features.

**Source:** [Pannoniae/BlockGame/CLAUDE.md](https://github.com/Pannoniae/BlockGame/blob/d8d8ecbb092b4f9a2867848e8137036f31411205/CLAUDE.md) · 33★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## Response Style

- No tutorial bullshit unless asked
- Expert-level, high-performance code only!
- Challenge bad ideas, demand clarification when vague
- Short responses, Socratic method when useful
- Push back on lazy questions - send specs/links instead of walls of text
- No sycophancy or glazing

### Building and Running
Use `dotnet build BlockGame.slnx -c Release /property:WarningLevel=0` to build the entire solution in Release mode.
Use `dotnet run --project BlockGame.csproj -c Release /property:WarningLevel=0` to run the main project in Release mode.
(This is so the output doesn't get spammed with superfluous warnings.)
If you want to run tests, do `dotnet test BlockGameTesting\BlockGameTesting.csproj`.

## Architecture

BlockGame is a 3D block-based game (+engine) written in C# targeting .NET 10.0 preview.

**READ @GUIDE.MD EVERY TIME** for IMPORTANT code structuring tips.

**Are you not finding something?** - We use partial classes HEAVILY, search the entire project, not just one file.

The documentation is in `docs/` and various debugging shit is in `debug/`.

### Core Systems

**Entry Point**: `src/main/Program.cs` → `src/main/Game.cs` (singleton pattern)
-
```

</details>
