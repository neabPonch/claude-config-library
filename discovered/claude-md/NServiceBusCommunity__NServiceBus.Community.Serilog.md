---
name: NServiceBusCommunity__NServiceBus.Community.Serilog
source: https://github.com/NServiceBusCommunity/NServiceBus.Community.Serilog/blob/bef1fbb9ab4eb3dd9d505db0aa184a02a08c2e49/claude.md
repo: NServiceBusCommunity/NServiceBus.Community.Serilog
kind: claude-md
stars: 41
last_pushed: 2026-06-15T22:37:55Z
license: mit
score: 9
domains: [backend, .net]
tags: [architecture, build-system, integration]
curated: 2026-06-16
curated_by: config-scout
---

# NServiceBusCommunity/NServiceBus.Community.Serilog — claude-md

**Why it's worth keeping:** Includes critical 'don't' warnings regarding auto-generated documentation and provides deep context on internal state management and exception enrichment logic.

**Summary:** A highly technical guide that explains not just how to build/test, but the underlying architectural mechanics and data flow of the library.

**Source credibility:** High; comes from an active, well-maintained community project for NServiceBus.

**Recency:** Current; uses modern .NET toolchains and specific test frameworks like TUnit.

**Source:** [NServiceBusCommunity/NServiceBus.Community.Serilog/claude.md](https://github.com/NServiceBusCommunity/NServiceBus.Community.Serilog/blob/bef1fbb9ab4eb3dd9d505db0aa184a02a08c2e49/claude.md) · 41★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Build and test

All projects live under `src/`. The SDK is pinned by `global.json` (`10.0.300`, `rollForward: latestFeature`, prerelease allowed). Tests use Microsoft.Testing.Platform (`UseMicrosoftTestingPlatformRunner`) via TUnit + Verify, not VSTest.

```pwsh
dotnet build src --configuration Release
dotnet test --solution src/NServiceBus.Serilog.sln --configuration Release --no-build --no-restore
```

Run a single test (TUnit / MTP filter syntax):

```pwsh
dotnet run --project src/Tests --configuration Debug -- --filter-method "*Handler"
```

Build settings to be aware of (`src/Directory.Build.props`):

- `TreatWarningsAsErrors=true` and `EnforceCodeStyleInBuild=true` — warnings and analyzer style violations fail the build.
- `LangVersion=preview`, `ImplicitUsings=enable`. Common namespaces (`NServiceBus.*`, `Serilog.*`, etc.) are injected as `<Using>` in the main csproj — don't add explicit `using` directives for those.
- Package versions are centralized in `src/Directory.Packages.props` (`ManagePackageVersionsCentrally=true`). Add version numbers there, not i
```

</details>
