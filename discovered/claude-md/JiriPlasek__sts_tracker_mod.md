---
name: JiriPlasek__sts_tracker_mod
source: https://github.com/JiriPlasek/sts_tracker_mod/blob/4f15c566b0666391004145a2a8f585b79dd0318b/CLAUDE.md
repo: JiriPlasek/sts_tracker_mod
kind: claude-md
stars: 3
last_pushed: 2026-04-15T00:39:50Z
license: unknown
score: 9
domains: [game-development, .net, modding]
tags: [csharp, godot, harmony-patches]
curated: 2026-06-16
curated_by: config-scout
---

# JiriPlasek/sts_tracker_mod — claude-md

**Why it's worth keeping:** It includes critical 'negative constraints'—explicit instructions on what the agent *cannot* do with Harmony patches or UI updates—to prevent common runtime failures.

**Summary:** Extremely high-quality technical documentation that outlines the specific architectural constraints and async timing nuances of a Godot/C# mod.

**Source credibility:** Low star count, but highly technical content suggests an expert-level developer.

**Recency:** Very current; uses modern .NET 9.0 and was updated recently.

**Source:** [JiriPlasek/sts_tracker_mod/CLAUDE.md](https://github.com/JiriPlasek/sts_tracker_mod/blob/4f15c566b0666391004145a2a8f585b79dd0318b/CLAUDE.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Project Overview
STS Tracker Companion Mod — a Slay the Spire 2 C# mod (Godot 4.5 / MegaDot, .NET 9.0) that shows card pick recommendations in-game and auto-uploads runs to [STS Tracker](https://ststracker.app). Published on [Nexus Mods](https://www.nexusmods.com/slaythespire2/mods/340).

## Architecture
- **Entry point**: `Plugin.cs` — `[ModInitializer]`, loads config, inits Harmony patches and ScoreOverlay.
- **Patches**: Harmony postfix patches on game screen classes to intercept card selection events. See Harmony Gotchas below.
- **UI**: `ScoreOverlay.cs` — singleton that creates Godot UI nodes (badges, tooltips) and attaches them to card holders.
- **HTTP**: `HttpService.cs` — async calls to STS Tracker API with Bearer token auth.
- **Config**: `sts_companion_config.cfg` (JSON) loaded from same directory as DLL.
- **Inspect tool**: `tools/` — decompilation utility for exploring game DLL APIs. Run with `dotnet run -- "Full.Type.Name"` or `dotnet run -- --search "keyword"`.

## Harmony Gotchas
- **Can't patch inherited methods on subclasses**: If a method isn't explicitly overridden by the subclass, Harmony can't find it. Patch the base class instead (e.g., `NCardGridSelection
```

</details>
