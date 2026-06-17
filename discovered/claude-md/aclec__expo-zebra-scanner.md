---
name: aclec__expo-zebra-scanner
source: https://github.com/aclec/expo-zebra-scanner/blob/72e2a9713f8bc6a4eff04e2046814252c00fabda/CLAUDE.md
repo: aclec/expo-zebra-scanner
kind: claude-md
stars: 27
last_pushed: 2026-05-22T16:09:25Z
license: unknown
score: 9
domains: [mobile-development, native-bridge]
tags: [architecture, expo, android-kotlin, ios-swift, api-contract]
curated: 2026-06-15
curated_by: config-scout
---

# aclec/expo-zebra-scanner — claude-md

**Why it's worth keeping:** The 'Behavioral Guarantees' section is world-class, documenting complex LIFO event dispatching that would otherwise be lost during refactoring. The 'Native Android rules' provide specific, actionable instructions for handling data serialization across the JSI bridge.

**Summary:** This file provides a comprehensive multi-layer architectural map covering JS, Android (Kotlin), and iOS layers. It explicitly defines the relationship between public APIs and internal native logic.

**Source credibility:** A specialized Expo module with recent maintenance activity.

**Recency:** Very current; aligns with modern Expo and React Native development patterns.

**Source:** [aclec/expo-zebra-scanner/CLAUDE.md](https://github.com/aclec/expo-zebra-scanner/blob/72e2a9713f8bc6a4eff04e2046814252c00fabda/CLAUDE.md) · 27★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

Guidance for Claude Code when working in this repository.

## Project purpose

`expo-zebra-scanner` is an Expo module exposing hook-based APIs for Zebra DataWedge.

- Android: full native support.
- iOS: compatibility stubs (no-op behavior).

Published as an npm package (`main: build/index.js`, `types: build/index.d.ts`); current version `56.0.0`.

## Architecture

### TypeScript / JS

- `src/index.ts`: public API exports (hooks + types only).
- `src/internal/constants.ts`: shared string constants (`DEFAULT_BARCODE_ACTION`, `DATAWEDGE_API_ACTION`).
- `src/internal/profile.ts`: profile creation and low-level broadcast helpers (`sendBroadcast`, `sendActionCommand`, `createIntentDatawedgeProfile`, `getDataWedgeVersion`) with runtime payload validation.
- `src/internal/zebraManager.ts`: singleton subscription manager with LIFO exclusive dispatch per action.
- `src/useZebraScanner.ts`: barcode-focused hook.
- `src/useZebraCustomScanner.ts`: raw custom-intent hook.
- `src/useZebraCreateProfile.ts`: profile creation hook (`useZebraCreateProfile`).
- `src/useZebraCoreFunctions.ts`: imperative core functions hook.

### Android (Kotlin)

Path: `android/src/main/java/expo/modules
```

</details>
