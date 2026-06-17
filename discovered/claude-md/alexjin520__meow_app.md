---
name: alexjin520__meow_app
source: https://github.com/alexjin520/meow_app/blob/ad90a1124771fdc0ba4760d6916733f1b65ad660/CLAUDE.md
repo: alexjin520/meow_app
kind: claude-md
stars: 2
last_pushed: 2025-06-10T01:36:17Z
license: unknown
score: 8
domains: [mobile-development, flutter]
tags: [flutter, android-native, live2d, architecture]
curated: 2026-06-17
curated_by: config-scout
---

# alexjin520/meow_app — claude-md

**Why it's worth keeping:** Excellent at documenting 'dark corners' like NDK versions, JNI bridges, and platform-specific build requirements. It uses specific command snippets to bridge high-level tasks with low-level execution.

**Summary:** Provides detailed architectural context for a Flutter app with complex Android-specific Live2D native integrations.

**Source credibility:** Low star count indicates a niche personal project rather than an industry standard.

**Recency:** Last updated 12 months ago; still highly relevant for current development workflows.

**Source:** [alexjin520/meow_app/CLAUDE.md](https://github.com/alexjin520/meow_app/blob/ad90a1124771fdc0ba4760d6916733f1b65ad660/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Cat App is a Flutter-based productivity application that combines task management with gamification through virtual cat companions. The app features Live2D animations (Android-only), customizable cat avatars, and a terminal-style task management interface.

## Essential Commands

### Development
```bash
# Install dependencies
flutter pub get

# Run the app in debug mode (default)
flutter run

# Run with specific device
flutter devices  # List available devices
flutter run -d <device_id>

# Clean build artifacts
flutter clean
```

### Testing
```bash
# Run all tests
flutter test

# Run specific test file
flutter test test/widget_test.dart

# Run tests with coverage
flutter test --coverage
```

### Building
```bash
# Android APK
flutter build apk --release

# Android App Bundle (for Play Store)
flutter build appbundle --release

# iOS (requires macOS with Xcode)
flutter build ios

# Web
flutter build web
```

### Code Quality
```bash
# Analyze code for issues
flutter analyze

# Format code
flutter format .
```

## Architecture Overview

### Navigat
```

</details>
