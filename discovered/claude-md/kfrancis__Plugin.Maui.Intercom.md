---
name: kfrancis__Plugin.Maui.Intercom
source: https://github.com/kfrancis/Plugin.Maui.Intercom/blob/b09fd67742d00234fd4c217effac0a66d65c82d1/CLAUDE.md
repo: kfrancis/Plugin.Maui.Intercom
kind: claude-md
stars: 2
last_pushed: 2026-01-22T16:12:11Z
license: mit
score: 9
domains: [.net, mobile-dev, cross-platform]
tags: [maui, android, ios, interop, build-commands]
curated: 2026-06-16
curated_by: config-scout
---

# kfrancis/Plugin.Maui.Intercom — claude-md

**Why it's worth keeping:** The breakdown of the Native Library Interop (NLI) pattern and platform-specific file suffixes is excellent; it prevents an LLM from getting lost in a complex cross-platform codebase.

**Summary:** Provides highly detailed build commands for multi-platform targets and explains complex native interop architecture.

**Source credibility:** Low star count, but high-quality technical documentation indicating a well-structured project.

**Recency:** Very current; references .NET 9.0 and recent AndroidX compatibility requirements.

**Source:** [kfrancis/Plugin.Maui.Intercom/CLAUDE.md](https://github.com/kfrancis/Plugin.Maui.Intercom/blob/b09fd67742d00234fd4c217effac0a66d65c82d1/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Plugin.Maui.Intercom is a .NET MAUI plugin that provides Intercom integration using Native Library Interop (NLI). It wraps the native Intercom SDK for Android and iOS/macOS platforms.

**Status**: Both Android and iOS platforms are working.

## Build Commands

```bash
# Build the main solution (includes binding projects and sample)
dotnet build src/Plugin.Maui.Intercom.sln -c Release

# Build Android-only
dotnet build src/Plugin.Maui.Intercom/Plugin.Maui.Intercom.csproj -c Release -f net9.0-android

# Build iOS-only (requires macOS)
dotnet build src/Plugin.Maui.Intercom/Plugin.Maui.Intercom.csproj -c Release -f net9.0-ios

# Run the sample app on Android
dotnet build src/sample/MauiSample.csproj -c Debug -f net9.0-android -t:Run

# Run the sample app on iOS (requires macOS)
dotnet build src/sample/MauiSample.csproj -c Debug -f net9.0-ios -t:Run
```

## Architecture

### Project Structure

- `src/Plugin.Maui.Intercom/` - Main MAUI plugin library (multi-targeted net9.0-android;net9.0-ios)
- `src/android/Intercom.Android.Binding/` - Android native b
```

</details>
