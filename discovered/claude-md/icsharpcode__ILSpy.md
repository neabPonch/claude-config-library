---
name: icsharpcode__ILSpy
source: https://github.com/icsharpcode/ILSpy/blob/c637fdbc847bc71a409d1ffa82332a3702554694/CLAUDE.md
repo: icsharpcode/ILSpy
kind: claude-md
stars: 25432
last_pushed: 2026-06-15T17:00:58Z
license: mit
score: 10
domains: [.net, cli-tools, desktop-app]
tags: [build-system, behavioral-guidelines, environment-safety]
curated: 2026-06-15
curated_by: config-scout
---

# icsharpcode/ILSpy — claude-md

**Why it's worth keeping:** Uses high-level behavioral constraints (e.g., preventing silent undoing of external edits) and explains the 'why' behind non-standard build scripts to prevent environment corruption.

**Summary:** Provides deep technical context for a complex .NET project, including specific tech stack nuances and critical git submodule management rules.

**Source credibility:** Extremely high; ILSpy is a major, widely-used open-source .NET decompiler with significant star count and active maintenance.

**Recency:** Very current; mentions cutting-edge technologies like net10.0/11.0 and Avalonia 12.

**Source:** [icsharpcode/ILSpy/CLAUDE.md](https://github.com/icsharpcode/ILSpy/blob/c637fdbc847bc71a409d1ffa82332a3702554694/CLAUDE.md) · 25432★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

Guidance for Claude Code (and future Claude sessions) when working on ILSpy.

## What this codebase is

ILSpy is a cross-platform .NET assembly browser / decompiler built on **Avalonia 12**, on top of the cross-platform `ICSharpCode.ILSpyX` and `ICSharpCode.Decompiler` core libraries.

## Tech stack

- **Avalonia 12** (not 11.x).
- **AvaloniaEdit** for the decompiled-code text view.
- **Dock** (wieslawsoltes/Dock) for the panel layout. NuGet id ≠ CLR namespace — `Dock.Controls.Recycling` lives in `Avalonia.Controls.Recycling`; decompile before guessing xmlns.
- **Avalonia.Xaml.Behaviors** for attached-behaviour glue.
- **Avalonia.ExtendedToolkit** (mameolan) for controls not in Avalonia core.
- **Simple** theme (not Fluent). Check `App.axaml` / csproj before assuming Fluent.
- **Microsoft.Extensions.DependencyInjection** + **System.Composition** MEF directly, with a small bridge.
- Central package management is enabled — every `PackageReference` needs a matching `PackageVersion` in `Directory.Packages.props`.
- Target framework: `net10.0` (cross-platform) for the main app. The test projects target `net11.0` (and `net11.0-windows` for tests that intentionally exercise W
```

</details>
