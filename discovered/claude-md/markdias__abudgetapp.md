---
name: markdias__abudgetapp
source: https://github.com/markdias/abudgetapp/blob/d55d3a020ae77c021c1fcfaada4c7e0eb913ede7/Claude.md
repo: markdias/abudgetapp
kind: claude-md
stars: 0
last_pushed: 2025-11-01T17:21:08Z
license: unknown
score: 9
domains: [ios, swiftui]
tags: [architecture-driven, build-automation, mvvm]
curated: 2026-06-17
curated_by: config-scout
---

# markdias/abudgetapp — claude-md

**Why it's worth keeping:** The breakdown of the 'Store Objects Pattern' explains exactly how state propagates through the app; includes ready-to-use xcodebuild command sets.

**Summary:** A highly detailed architectural guide for a SwiftUI app that focuses on actor-based concurrency and data persistence patterns.

**Source credibility:** Small personal repository, but exhibits professional-grade documentation standards.

**Recency:** Current, mentioning Swift 6 and Xcode 15+ requirements.

**Source:** [markdias/abudgetapp/Claude.md](https://github.com/markdias/abudgetapp/blob/d55d3a020ae77c021c1fcfaada4c7e0eb913ede7/Claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Guidelines

1. **Always update this claude.md when significant changes are made** – Keep architectural descriptions in sync with implementation.
2. **Always ask clarifying questions** – Confirm intent before major refactors or feature additions.
3. **Do not test the build** – Avoid running Xcode builds during development (user manages testing).
4. **Use absolute code references** – When discussing code, use format `file.swift:123` or markdown links like `[file.swift:123](path/file.swift#L123)`.

## Build & Run Commands

**Build the app:**
```bash
xcodebuild build -scheme abudgetapp -configuration Debug
```

**Run on simulator:**
```bash
xcodebuild build-for-testing -scheme abudgetapp -destination 'platform=iOS Simulator,name=iPhone 15'
```

**Run UI tests:**
```bash
xcodebuild test -scheme abudgetapp -destination 'platform=iOS Simulator,name=iPhone 15'
```

**Run specific test:**
```bash
xcodebuild test -scheme abudgetapp -testProductName abudgetappUITests \
  -destination 'platform=iOS Simulator,name=iPhone 15'
```

**Clean build:**
```bash
xcodebuild
```

</details>
