---
name: Cleric-K__vJoySerialFeeder
source: https://github.com/Cleric-K/vJoySerialFeeder/blob/0cfbdca9cbba8d9e8f6d3c67f5b3462050953655/CLAUDE.md
repo: Cleric-K/vJoySerialFeeder
kind: claude-md
stars: 284
last_pushed: 2026-03-31T16:09:13Z
license: gpl-3.0
score: 9
domains: [desktop-app, .net]
tags: [.net, windows-forms, cross-platform]
curated: 2026-06-15
curated_by: config-scout
---

# Cleric-K/vJoySerialFeeder — claude-md

**Why it's worth keeping:** The 'Key architecture notes' section provides essential context on technical debt (singletons/UI coupling) which prevents the AI from making bad assumptions. The explicit directory breakdown is also a high-value pattern for complex legacy projects.

**Summary:** A highly technical development guide providing specific build commands, project structure mapping, and architectural intent.

**Source credibility:** High; it is an established open-source project with recent maintenance activity.

**Recency:** Current; includes future-looking modernization roadmaps and platform-specific nuances.

**Source:** [Cleric-K/vJoySerialFeeder/CLAUDE.md](https://github.com/Cleric-K/vJoySerialFeeder/blob/0cfbdca9cbba8d9e8f6d3c67f5b3462050953655/CLAUDE.md) · 284★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# vJoySerialFeeder — Development Guide

## What is this project?

A Windows Forms application (.NET Framework 4.8) that reads serial data from RC controller protocols (IBUS, SBUS, CRSF, DSM, etc.) and maps it to virtual joystick devices (vJoy, vXbox on Windows; uinput on Linux via Mono). Licensed under GPLv3.

## Build

```bash
# Windows (requires MSBuild / Visual Studio Build Tools)
msbuild vJoySerialFeeder/vJoySerialFeeder.sln /p:Configuration=Release /p:Platform="Any CPU"

# Linux (requires Mono)
xbuild vJoySerialFeeder/vJoySerialFeederLinux.csproj /p:Configuration=Release
```

## Test

```bash
dotnet test vJoySerialFeeder.Tests/
```

## Project structure

```
vJoySerialFeeder/
  MainForm.cs, MainFormWorker.cs    — Main UI and worker loop
  Configuration.cs                  — Profile/settings management (JSON serialization)
  SerialProtocols/                  — Protocol readers (IBUS, SBUS, DSM, CRSF, etc.)
  Mappings/                         — Channel-to-joystick mapping (axis, button, bitmap)
  VirtualJoysticks/                 — Platform-abstracted joystick drivers
  Scripting/                        — Lua scripting engine (MoonSharp)
  ProcessInteraction/               — COM
```

</details>
