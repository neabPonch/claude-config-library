---
name: sander1095__soundtouch-maui
source: https://github.com/sander1095/soundtouch-maui/blob/59a0621a74b3a8dcf4c93239ff4d6534f2e3c4ca/CLAUDE.md
repo: sander1095/soundtouch-maui
kind: claude-md
stars: 2
last_pushed: 2026-06-10T22:26:17Z
license: agpl-3.0
score: 9
domains: [.net-maui, mobile-dev, iot]
tags: [build-scripts, architecture-mapping, platform-specific]
curated: 2026-06-16
curated_by: config-scout
---

# sander1095/soundtouch-maui — claude-md

**Why it's worth keeping:** Uses an 'Architecture' section to explain specific communication protocols (WebSocket subprotocols) and provides critical developer-centric 'Conventions' for UI automation readiness.

**Summary:** Provides platform-specific build commands and a high-density architectural map of service interactions.

**Source credibility:** Niche personal project with high-quality documentation structure.

**Recency:** Extremely current; updated within the last month.

**Source:** [sander1095/soundtouch-maui/CLAUDE.md](https://github.com/sander1095/soundtouch-maui/blob/59a0621a74b3a8dcf4c93239ff4d6534f2e3c4ca/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

### Build

```bash
# Mac Catalyst (primary dev target)
dotnet build src/SoundTouch.Maui/SoundTouchMaui.csproj -f net10.0-maccatalyst /p:_RequireCodeSigning=false
open src/SoundTouch.Maui/bin/Debug/net10.0-maccatalyst/maccatalyst-arm64/AfterTouch.app

# iOS simulator
dotnet build src/SoundTouch.Maui/SoundTouchMaui.csproj -f net10.0-ios -p:RuntimeIdentifier=iossimulator-arm64

# Android (EmbedAssembliesIntoApk bypasses Fast Deploy for sideloading)
dotnet build src/SoundTouch.Maui/SoundTouchMaui.csproj -f net10.0-android -p:EmbedAssembliesIntoApk=true

# Speaker emulator (HTTP :8090, WebSocket :8080 — matches real speaker defaults)
dotnet run --project src/SoundTouchMaui.Emulator
```

### Tests

```bash
# Unit tests (fast, runs on any OS)
dotnet test tests/SoundTouchMaui.Tests

# Single unit test
dotnet test tests/SoundTouchMaui.Tests --filter "FullyQualifiedName~TestClassName.MethodName"
```

> End-to-end UI tests (Appium) are not part of v1 — that work lives on the
> `ui-tests-v2` branch.

### Formatting

```bash
dotnet tool restore          # restore csh
```

</details>
