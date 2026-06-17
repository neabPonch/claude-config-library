---
name: kadikraman__do-you-remember__expo-ui-skill
source: https://github.com/kadikraman/do-you-remember/blob/8a4edff25445c46a7698ba5baf47fc18164a7090/expo-ui-skill.md
repo: kadikraman/do-you-remember
kind: skill
stars: 2
last_pushed: 2026-05-19T18:20:04Z
license: unknown
score: 9
domains: [mobile-dev, react-native, ios, android]
tags: [expo, swiftui, jetpack-compose, ui-library]
curated: 2026-06-16
curated_by: config-scout
---

# kadikraman/do-you-remember — skill

**Why it's worth keeping:** The documentation emphasizes critical architecture details like the mandatory 'Host' wrapper and provides dense, machine-readable prop tables that prevent syntax hallucinations.

**Summary:** A highly structured API reference for the @expo/ui library, enabling agents to implement native SwiftUI and Jetpack Compose components within React Native.

**Source credibility:** High technical density; though star count is low, the specificity of SDK versions suggests specialized expertise.

**Recency:** Very recent, referencing Expo SDK 54/55 and modern native primitives.

**Source:** [kadikraman/do-you-remember/expo-ui-skill.md](https://github.com/kadikraman/do-you-remember/blob/8a4edff25445c46a7698ba5baf47fc18164a7090/expo-ui-skill.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Expo UI Skill

## Overview

`@expo/ui` brings native SwiftUI (iOS/tvOS/macOS) and Jetpack Compose (Android) components to React Native via Expo. It is NOT a JS UI library — it exposes real native platform primitives directly to JavaScript.

- **Package:** `@expo/ui`
- **Install:** `npx expo install @expo/ui`
- **Requires:** Development build (not Expo Go)
- **Available since:** SDK 54 (SwiftUI focus), SDK 55 (expanded Jetpack Compose)

Two separate import paths:
- `@expo/ui/swift-ui` — iOS/tvOS/macOS components
- `@expo/ui/swift-ui/modifiers` — SwiftUI modifiers
- `@expo/ui/jetpack-compose` — Android components
- `@expo/ui/jetpack-compose/modifiers` — Jetpack Compose modifiers

## Critical Concept: The Host Component

`Host` is **required** as the root container to bridge from React Native (UIKit/Android Views) into SwiftUI/Jetpack Compose. Think of it like `<svg>` in HTML or `<Canvas>` in react-native-skia.

```tsx
import { Host, Text } from '@expo/ui/swift-ui';

// Host wraps SwiftUI content — style it with RN styles
<Host style={{ flex: 1 }}>
  <Text>Hello SwiftUI</Text>
</Host>

// matchContents makes Host shrink to fit its SwiftUI content
<Host matchContents>
  <Text>Sized t
```

</details>
