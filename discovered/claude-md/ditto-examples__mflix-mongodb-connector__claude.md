---
name: ditto-examples__mflix-mongodb-connector__claude
source: https://github.com/ditto-examples/mflix-mongodb-connector/blob/ac52e1b09f3b547b044fb9b53f64de6c8ef1fdfe/swift/Claude.md
repo: ditto-examples/mflix-mongodb-connector
kind: claude-md
stars: 3
last_pushed: 2025-11-21T21:18:09Z
license: apache-2.0
score: 8
domains: [ios-development, swiftui]
tags: [swiftui, @observable, modern-architecture]
curated: 2026-06-16
curated_by: config-scout
---

# ditto-examples/mflix-mongodb-connector — claude-md

**Why it's worth keeping:** It explicitly forbids legacy protocols (like ObservableObject) and provides exact replacement patterns for state management to prevent technical debt/code regression.

**Summary:** Defines strict architectural constraints for a modern SwiftUI project using the new @Observable macro pattern.

**Source credibility:** High; provided by an official sample application from the Ditto team.

**Recency:** Very current; specifically addresses iOS 17+, macOS 14, and Swift 6 compatibility.

**Source:** [ditto-examples/mflix-mongodb-connector/swift/Claude.md](https://github.com/ditto-examples/mflix-mongodb-connector/blob/ac52e1b09f3b547b044fb9b53f64de6c8ef1fdfe/swift/Claude.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# MFlix Movies - Swift iOS App

## Project Overview
This is a SwiftUI-based iOS application that connects to a MongoDB database through Ditto to display and manage movie information. The app provides a modern, native iOS interface for browsing movies, searching content, viewing details, managing movie data, monitoring sync status, and tracking database indexes.

### Modern Swift & Observable Macro Architecture
This project has been fully migrated to use the new **@Observable macro API** introduced in iOS 17/macOS 14, replacing the legacy ObservableObject protocol. All observable classes use the modern pattern for better performance and cleaner code.

**Key Architecture Decisions:**
- Uses `@Observable` macro for all observable classes (no ObservableObject)
- Leverages `@Environment` instead of @EnvironmentObject
- Uses `@State` for Observable class instances (not @StateObject)
- No `@Published` property wrappers needed
- Full Swift 6 compatibility with proper concurrency handling

**Platform Requirements:**
- **Minimum iOS Version**: 17.0
- **Minimum macOS Version**: 14.0
- **Swift Version**: 5.0+ (with @Observable macro support)
- **Swift 6 Ready**: No concurrency warnings or comp
```

</details>
