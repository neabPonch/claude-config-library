---
name: piemonte__Burst
source: https://github.com/piemonte/Burst/blob/dc817dd72385a7a6e1f3e3e997d0b8be31e9d656/CLAUDE.md
repo: piemonte/Burst
kind: claude-md
stars: 31
last_pushed: 2026-01-21T06:54:57Z
license: mit
score: 8
domains: [ios, swift]
tags: [mobile-dev, ui-components, xcode]
curated: 2026-06-15
curated_by: config-scout
---

# piemonte/Burst — claude-md

**Why it's worth keeping:** The use of line-number annotations (e.g., 'Sources/Burst.swift:31-163') is a pro technique that allows Claude to jump straight to relevant definitions. It also documents the internal logic flow (two-phase animation) which aids architectural reasoning.

**Summary:** Provides specific build commands and maps core components to exact file-line ranges.

**Source credibility:** Small, focused open-source library with specific documentation standards.

**Recency:** Current; uses modern Xcode/Swift build workflows compatible with current tools.

**Source:** [piemonte/Burst/CLAUDE.md](https://github.com/piemonte/Burst/blob/dc817dd72385a7a6e1f3e3e997d0b8be31e9d656/CLAUDE.md) · 31★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Common Development Commands

### Building the project
```bash
# Build using Xcode
xcodebuild -workspace Burst.xcworkspace -scheme 'Debug - iOS' -sdk iphonesimulator build

# Build release version
xcodebuild -workspace Burst.xcworkspace -scheme 'Release - iOS' -sdk iphonesimulator build
```

### Testing
```bash
# Run tests (if test target exists)
xcodebuild -workspace Burst.xcworkspace -scheme 'Debug - iOS' -sdk iphonesimulator test

# Analyze code for issues
xcodebuild -workspace Burst.xcworkspace -scheme 'Debug - iOS' -sdk iphonesimulator analyze
```

### Package Management
```bash
# CocoaPods - install/update dependencies
pod install

# Swift Package Manager - build the package
swift build

# Swift Package Manager - test the package
swift test
```

## Architecture and Structure

Burst is a Swift iOS library that provides a firework burst effect using CAEmitterLayers. The library is designed to be simple and easy to integrate.

### Core Components

#### BurstView (Sources/Burst.swift:31-163)
- UIView subclass that manages the burst animation effect
- Uses two CAE
```

</details>
