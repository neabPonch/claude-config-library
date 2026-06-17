---
name: ExpTechTW__DPIP
source: https://github.com/ExpTechTW/DPIP/blob/789f5f18f8c91cf54963843cb402589b83990ea2/CLAUDE.md
repo: ExpTechTW/DPIP
kind: claude-md
stars: 249
last_pushed: 2026-06-15T02:04:30Z
license: other
score: 9
domains: [mobile-app, flutter]
tags: [flutter, dart, coding-standards, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# ExpTechTW/DPIP — claude-md

**Why it's worth keeping:** The 'Key Conventions' section is exceptional, providing specific rules for class member ordering and project-specific context extensions to minimize boilerplate. This ensures the AI produces idiomatic code rather than generic Dart.

**Summary:** A comprehensive guide for a Flutter application that covers build commands, architectural layout, and highly granular coding standards.

**Source credibility:** High; part of a real-world disaster prevention project with significant GitHub stars and active maintenance.

**Recency:** Very current, utilizing modern Flutter patterns like Material 3 and specific GoRouter implementations.

**Source:** [ExpTechTW/DPIP/CLAUDE.md](https://github.com/ExpTechTW/DPIP/blob/789f5f18f8c91cf54963843cb402589b83990ea2/CLAUDE.md) · 249★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

DPIP (Disaster Prevention Information Platform) — a Flutter app for Taiwan earthquake early warning and disaster information, integrating TREM-Net and CWA data.

## Commands

```bash
# Install dependencies
flutter pub get --no-example

# Format
dart format .

# Lint
dart analyze .

# Code generation (required after editing routes, @JsonSerializable, or @freezed models)
dart run build_runner build

# Update translations
bash tools/update_translations.sh

# Run
flutter run

# Build
flutter build apk --release
flutter build ios --release
```

There is no test suite.

## Architecture

**State management:** Provider (`ChangeNotifier`). Global providers are registered in `lib/core/providers.dart`:
- `DpipDataModel` — earthquake/weather data
- `SettingsLocationModel`, `SettingsMapModel`, `SettingsNotificationModel`, `SettingsUserInterfaceModel`

**Routing:** go_router with type-safe routes via `@TypedGoRoute`. Routes are defined in `router.dart` and code-generated into `router.g.dart`. Run `build_runner` after route changes.

**Feature modules** live under `lib/
```

</details>
