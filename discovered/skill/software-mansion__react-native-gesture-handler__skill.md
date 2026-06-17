---
name: software-mansion__react-native-gesture-handler__skill
source: https://github.com/software-mansion/react-native-gesture-handler/blob/a70c6e3496af859260f06b06ccb9ef2df2394b91/skills/gesture-handler-3-migration/SKILL.md
repo: software-mansion/react-native-gesture-handler
kind: skill
stars: 6753
last_pushed: 2026-06-14T02:19:43Z
license: mit
score: 9
domains: [mobile, react-native]
tags: [migration, refactoring, gestures]
curated: 2026-06-15
curated_by: config-scout
---

# software-mansion/react-native-gesture-handler — skill

**Why it's worth keeping:** Provides exact mapping rules for API changes, callback renaming, and complex architectural shifts like SVG hierarchy handling. The inclusion of specific code examples for logic inversion (success vs canceled) is a top-tier technique for AI accuracy.

**Summary:** A highly detailed migration guide for upgrading react-native-gesture-handler from version 2 to 3.

**Source credibility:** High; sourced from a major industry-standard library with significant community maintenance.

**Recency:** Modern; specifically addresses version 3 of the library.

**Source:** [software-mansion/react-native-gesture-handler/skills/gesture-handler-3-migration/SKILL.md](https://github.com/software-mansion/react-native-gesture-handler/blob/a70c6e3496af859260f06b06ccb9ef2df2394b91/skills/gesture-handler-3-migration/SKILL.md) · 6753★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: gesture-handler-3-migration
description: Migrates files containing React Native components which use the React Native Gesture Handler 2 API to Gesture Handler 3.
---

# Migrate to Gesture Handler 3

This skill scans React Native components that use the Gesture Handler builder-based API and updates them to use the new hook-based API. It also updates related types and components to adapt to the new version.

## When to Use

- Updating the usage of components imported from `react-native-gesture-handler`
- Upgrading to Gesture Handler 3
- Migrating to the new hook-based gesture API

## Instructions

Use the instructions below to correctly replace all legacy APIs with the modern ones.

1. Identify all imports from 'react-native-gesture-handler'
2. For each `Gesture.X()` call, replace with corresponding `useXGesture()` hook
3. Replace `Gesture` import with imports for the used hooks
4. Convert builder method chains to configuration objects
5. Update callback names (onStart → onActivate, etc.)
6. Replace composed gestures with relation hooks. Keep rules of hooks in mind
7. Update GestureDetector usage if SVG is involved to Intercepting/Virtual GestureDetector
8. Update usage of
```

</details>
