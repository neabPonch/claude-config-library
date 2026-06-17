---
name: getsentry__sentry-unreal
source: https://github.com/getsentry/sentry-unreal/blob/3f7f1f3859f0491fd4122f21c1f144b1bc1359b6/CLAUDE.md
repo: getsentry/sentry-unreal
kind: claude-md
stars: 164
last_pushed: 2026-06-15T18:47:31Z
license: mit
score: 9
domains: [game-development, sdk, c++]
tags: [unreal-engine, cross-platform, architecture]
curated: 2026-06-16
curated_by: config-scout
---

# getsentry/sentry-unreal — claude-md

**Why it's worth keeping:** Uses visual tree structures to explain multi-layered inheritance patterns and explicitly documents environmental variables/setup scripts necessary for specialized console development.

**Summary:** Provides a comprehensive architectural blueprint of a complex C++ Unreal Engine plugin, including platform hierarchies and build requirements.

**Source credibility:** High; official Sentry SDK repository with high star count and recent maintenance.

**Recency:** Current; last pushed within the current month.

**Source:** [getsentry/sentry-unreal/CLAUDE.md](https://github.com/getsentry/sentry-unreal/blob/3f7f1f3859f0491fd4122f21c1f144b1bc1359b6/CLAUDE.md) · 164★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This project is the Sentry SDK for Unreal Engine which provides crash and error monitoring as well as performance tracking for games built with Unreal Engine. It wraps multiple Sentry SDKs for supported platforms (`sentry-native` for Windows/Linux/macOS/Xbox/WinGDK/PlayStation/Nintendo, `sentry-cocoa` for macOS/iOS, `sentry-java` for Android) into a single Unreal Engine plugin and extends them with Unreal Engine-specific functionality.

## Plugin Architecture

### Plugin Modules

1. **Sentry** - Main plugin API with platform-specific implementations (Runtime module)
2. **SentryEditor** - Editor utilities, settings UI, build tools (Editor module)

### Plugin Source Structure

```
plugin-dev/Source/
├── Sentry/
│   ├── Public/              # Public API headers (SentrySubsystem.h, SentrySettings.h, SentryLibrary.h)
│   └── Private/
│       ├── Android/         # Android implementation (sentry-java via JNI)
│       ├── Apple/           # Base for Mac and iOS (sentry-cocoa)
│       ├── GenericPlatform/ # Base for Microsoft, Linux, PS, Switch (sentry-n
```

</details>
