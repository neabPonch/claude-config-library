---
name: anthony1810__ScreenStateKit__ssk-skill
source: https://github.com/anthony1810/ScreenStateKit/blob/2c988d5eebfb9e849959121b621cd7f1434cfb9e/ssk-skill.md
repo: anthony1810/ScreenStateKit
kind: skill
stars: 59
last_pushed: 2026-06-08T12:09:35Z
license: unknown
score: 8
domains: [ios, swiftui]
tags: [architecture, state-management, concurrency]
curated: 2026-06-15
curated_by: config-scout
---

# anthony1810/ScreenStateKit — skill

**Why it's worth keeping:** It offers highly specific patterns for de-duplicating concurrent actions via ActionLocker and batching state updates with animation control using updateState. The inclusion of parent-child state binding and load-more templates makes it an excellent architectural blueprint.

**Summary:** Defines the 'Three Pillars' architecture for managing SwiftUI screens through State, Store (Actor), and View components. It provides specialized logic for pagination, error propagation, and thread-safe action processing.

**Source credibility:** The 59-star repo suggests a specialized, well-regarded utility for SwiftUI developers.

**Recency:** Highly current; utilizes modern Swift Observation and iOS 17+ concurrency patterns.

**Source:** [anthony1810/ScreenStateKit/ssk-skill.md](https://github.com/anthony1810/ScreenStateKit/blob/2c988d5eebfb9e849959121b621cd7f1434cfb9e/ssk-skill.md) · 59★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# ScreenStateKit Skill

Use this skill when building features in Swift apps that use ScreenStateKit for state management. ScreenStateKit provides the "Three Pillars" pattern: **State** (Observable) + **Store** (Actor ViewModel) + **View** (SwiftUI). Use it for creating screens with loading states, error handling, pagination, action deduplication, async streaming, task cancellation, and CRUD environment callbacks.

## Requirements

- iOS 17+ / macOS 14+
- Swift 5.9+
- Swift Package: `https://github.com/anthony1810/ScreenStateKit.git`

## Architecture: The Three Pillars

Every feature has three components:

1. **State** (`ScreenState` subclass) - `@Observable @MainActor` class holding all UI data
2. **Store** (actor conforming to `ScreenActionStore`) - Processes actions, updates state
3. **View** (SwiftUI) - Binds state, dispatches actions to store

The flow: **View** dispatches actions to **Store** via `nonisolatedReceive(action:)` → framework's `dispatch` handles loading/error → **Store**'s `receive(action:) async throws` processes action → **Store** updates **State** → **View** re-renders via `@Observable`.

---

## Pillar 1: State

### Basic ScreenState

```swift
import ScreenSta
```

</details>
