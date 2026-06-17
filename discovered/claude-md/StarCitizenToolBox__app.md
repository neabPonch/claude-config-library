---
name: StarCitizenToolBox__app
source: https://github.com/StarCitizenToolBox/app/blob/fbb93d7f3f8ef2e44b9d51f986106d829f6a47f5/Claude.md
repo: StarCitizenToolBox/app
kind: claude-md
stars: 134
last_pushed: 2026-06-15T00:35:25Z
license: gpl-3.0
score: 9
domains: [desktop-app, flutter, rust]
tags: [architecture-guide, build-automation, cross-language]
curated: 2026-06-16
curated_by: config-scout
---

# StarCitizenToolBox/app — claude-md

**Why it's worth keeping:** Includes critical 'never cancel' build warnings for long processes and provides a clear mental model of the Rust-to-Dart bridge relationship.

**Summary:** A highly detailed guide covering complex build orchestration, multi-layer architecture (Rust/Dart), and specific warnings against editing generated files.

**Source credibility:** High; reflects a complex, real-world cross-language project with active maintenance.

**Recency:** Current; includes specific versions for modern toolchains like flutter_rust_bridge 2.12.0.

**Source:** [StarCitizenToolBox/app/Claude.md](https://github.com/StarCitizenToolBox/app/blob/fbb93d7f3f8ef2e44b9d51f986106d829f6a47f5/Claude.md) · 134★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

StarCitizenToolBox ("SC汉化盒子") — Flutter + Rust desktop app for Star Citizen players. Provides game localization, diagnostics, performance optimization, P4K archive browsing, audio playback, and more. Windows primary platform; Linux/macOS limited.

Package name: `starcitizen_doctor` (v3.1.1+81). Published on Microsoft Store via MSIX packaging.

## Build Commands

**Quick validation (5-10 min):**
```bash
flutter analyze && cd rust && cargo check
```

**Full build (45-60 min — NEVER CANCEL):**
```bash
flutter pub get
dart run build_runner build --delete-conflicting-outputs
cd rust && cargo update && cd ..
flutter_rust_bridge_codegen generate
flutter pub global activate intl_utils
flutter pub global run intl_utils:generate
flutter build windows -v
```

**Code generation (run after relevant changes):**
```bash
dart run build_runner build --delete-conflicting-outputs  # Dart model changes
flutter_rust_bridge_codegen generate                       # Rust API signature changes
flutter pub global run intl_utils:generate                 # Localization stri
```

</details>
