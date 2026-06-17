---
name: emerysilb__immibridge
source: https://github.com/emerysilb/immibridge/blob/0cbc0363af010e11c7dc9f0189214350fe164c7a/CLAUDE.md
repo: emerysilb/immibridge
kind: claude-md
stars: 307
last_pushed: 2026-04-23T04:15:47Z
license: mit
score: 9
domains: [macOS, swiftui]
tags: [macos, swiftui, architecture-map, build-automation]
curated: 2026-06-15
curated_by: config-scout
---

# emerysilb/immibridge — claude-md

**Why it's worth keeping:** It maps file sizes to responsibilities (e.g., ~3,600 lines) to help Claude navigate large files, and explicitly details data flow/entitlements which are critical for debugging sandbox issues.

**Summary:** A high-quality guide for a macOS SwiftUI project that bridges the gap between build instructions and architectural understanding.

**Source credibility:** High-quality open source project with 307 stars and a professional release workflow.

**Recency:** 

**Source:** [emerysilb/immibridge/CLAUDE.md](https://github.com/emerysilb/immibridge/blob/0cbc0363af010e11c7dc9f0189214350fe164c7a/CLAUDE.md) · 307★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

ImmiBridge is a native macOS app (SwiftUI) for backing up Apple Photos to local folders (organized by date) or to Immich photo servers. It supports incremental/full/mirror backup modes, pause/resume, scheduled backups, and menu bar integration. Auto-updates via Sparkle.

## Build Commands

**Open in Xcode:**
```bash
open ImmiBridge/ImmiBridge.xcodeproj
```

**Build from command line:**
```bash
./scripts/build_ui_app_bundle.sh
# Output: build/ImmiBridge.app
```

**Build with xcodebuild directly:**
```bash
xcodebuild -project ImmiBridge/ImmiBridge.xcodeproj -scheme ImmiBridge -configuration Release build
```

**Create signed/notarized release DMG** (requires `.env` with signing credentials, see `.env.example`):
```bash
./scripts/release.sh
```

**Generate Sparkle appcast:**
```bash
./scripts/generate_appcast.sh
```

There are no linters or automated test suites in active use. Testing is manual — run the app and exercise backup workflows.

## Architecture

**Pattern:** MVVM with SwiftUI. Views observe `PhotoBackupViewModel` via `@EnvironmentObject`.
```

</details>
