---
name: iSapozhnik__NimbusUI
source: https://github.com/iSapozhnik/NimbusUI/blob/436cf01f3cd47b97c073e8eb4377ed8b80f6ea00/CLAUDE.md
repo: iSapozhnik/NimbusUI
kind: claude-md
stars: 14
last_pushed: 2025-10-05T16:29:02Z
license: unknown
score: 9
domains: [swiftui, design-systems]
tags: [architecture-rules, ios-macos, component-library]
curated: 2026-06-15
curated_by: config-scout
---

# iSapozhnik/NimbusUI — claude-md

**Why it's worth keeping:** The 'Modifier-First Architecture Guidelines' provide clear constraints on how new components should be implemented to ensure consistency. The evaluation checklist is a highly effective technique for directing AI reasoning.

**Summary:** Provides deep architectural context and strict implementation guidelines for a SwiftUI component library. It includes specific build/test commands to facilitate automated verification.

**Source credibility:** A moderately starred SwiftUI library with professional, high-quality documentation.

**Recency:** Highly relevant for current development workflows involving modern Swift and SwiftUI.

**Source:** [iSapozhnik/NimbusUI/CLAUDE.md](https://github.com/iSapozhnik/NimbusUI/blob/436cf01f3cd47b97c073e8eb4377ed8b80f6ea00/CLAUDE.md) · 14★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

NimbusUI is a modular SwiftUI component library for macOS 14.0+ applications, built with Swift Package Manager. It provides a comprehensive theming system, reusable UI components, and custom view modifiers through four main libraries that can be imported selectively or as a complete umbrella package.

## Development Commands

### Build and Test
```bash
# Build the package
swift build

# Run tests (Swift Testing framework)
swift test

# Run specific test targets
swift test --filter NimbusCoreTests
swift test --filter NimbusComponentsTests  
swift test --filter NimbusNotificationsTests
swift test --filter NimbusOnboardingTests
swift test --filter NimbusBezelsTests

# Clean build artifacts
swift package clean

# Resolve dependencies
swift package resolve

# Update snapshots when needed
swift test -Xswiftc -DUPDATE_SNAPSHOTS
```

### Modular Library Structure
NimbusUI is organized into five distinct libraries for selective importing:

- **`NimbusCore`**: Core theming system, modifiers, utilities, and AppKit integrations
- **`NimbusComponents`**: Main
```

</details>
