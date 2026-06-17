---
name: svermeulen__trecs
source: https://github.com/svermeulen/trecs/blob/12fe09950f341550ac72aec94906eb1d3c89057b/CLAUDE.md
repo: svermeulen/trecs
kind: claude-md
stars: 80
last_pushed: 2026-06-05T06:43:11Z
license: mit
score: 8
domains: [game-dev, unity]
tags: [ecs, csharp, source-gen]
curated: 2026-06-15
curated_by: config-scout
---

# svermeulen/trecs — claude-md

**Why it's worth keeping:** Uses exact CLI commands for toolchains and defines low-level architectural constraints (e.g., unmanaged structs) that prevent incorrect code generation.

**Summary:** Provides specific build/test workflows for a multi-part system (Unity + SourceGen) and enforces domain-specific ECS coding patterns.

**Source credibility:** Decent niche popularity with very active maintenance.

**Recency:** Highly current, referencing modern Unity versions and C# tooling.

**Source:** [svermeulen/trecs/CLAUDE.md](https://github.com/svermeulen/trecs/blob/12fe09950f341550ac72aec94906eb1d3c89057b/CLAUDE.md) · 80★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
## Build

**Main project (Unity):**
Open `UnityProject/Trecs/Trecs.sln` in Unity 6000.3.10f1+ or your IDE.

**Source generator:**
```bash
dotnet build SourceGen/Trecs.SourceGen/Trecs.SourceGen.sln -c Release
```

To rebuild and install the source generator DLL into the Unity project:
```bash
cd SourceGen/Trecs.SourceGen && ./build_and_install.sh
```

## Tests

Run tests via Unity Test Runner (Window > General > Test Runner) in **EditMode**.

## Code Style

Uses [CSharpier](https://csharpier.com/) for formatting:
```bash
cd UnityProject/Trecs && dotnet tool restore && dotnet csharpier .
```

## Project Structure

- `UnityProject/Trecs/Assets/com.trecs.core/` - Core ECS library
- `UnityProject/Trecs/Assets/Trecs.Tests/` - Unit tests (editor-only)
- `UnityProject/Trecs/Assets/Samples/` - Sample projects
- `SourceGen/Trecs.SourceGen/` - Roslyn source generator

## Conventions

- Components are unmanaged structs implementing `IEntityComponent`
- Tags are marker structs implementing `ITag`
- Entity templates implement `ITemplate` with `ITags<>` and field declarations
- Systems implement `ISystem` or `IJobSystem`
- Namespaces follow folder structure under `Trecs` / `Trecs.Internal`
```

</details>
