---
name: keybase__client__skill
source: https://github.com/keybase/client/blob/ee3660551bbc1702a67b8a188679e1a54947b724/skill/prod-bundles/SKILL.md
repo: keybase/client
kind: skill
stars: 9220
last_pushed: 2026-06-12T23:12:47Z
license: bsd-3-clause
score: 9
domains: [frontend, mobile, build-systems]
tags: [webpack, metro, tree-shaking, bundle-audit, cross-platform]
curated: 2026-06-15
curated_by: config-scout
---

# keybase/client — skill

**Why it's worth keeping:** Includes highly specific verification techniques, such as a Python one-liner to check for global variable inlining and manual checks for module presence in production bundles.

**Summary:** Provides specific build commands and automated audit scripts to verify tree-shaking and variable inlining across desktop and mobile platforms.

**Source credibility:** High; source is the Keybase client, a major established open-source project.

**Recency:** Very current; repository shows extremely active maintenance.

**Source:** [keybase/client/skill/prod-bundles/SKILL.md](https://github.com/keybase/client/blob/ee3660551bbc1702a67b8a188679e1a54947b724/skill/prod-bundles/SKILL.md) · 9220★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: prod-bundles
description: Use when the user asks to build production bundles, check bundle sizes, audit tree-shaking, or verify mobile/desktop code separation. Covers both the desktop webpack prod build and the iOS/Android Metro bundle.
---

Build production bundles for both platforms and analyze them for correct tree-shaking.

## Build Commands

**Desktop (webpack):**
```bash
# From shared/
yarn desktop:build:prod
```
Output lands in `shared/desktop/dist/`. Prod bundles have no `.dev` or `.profile` suffix — filter with:
```bash
ls shared/desktop/dist/*.bundle.js | grep -v '\.dev\.' | grep -v '\.profile\.'
```

**iOS (Metro):**
```bash
# From shared/
yarn ios:jsbundle
```
Output: `shared/ios/dist/main.jsbundle`

**Android (Metro):**
```bash
# From shared/
yarn android:jsbundle
```
Output: `shared/android/dist/main.jsbundle`

## Tree-Shaking Audit

**Desktop — check mobile-only modules are absent:**
```bash
DIST=shared/desktop/dist
PROD=$(ls "$DIST"/*.bundle.js | grep -v '\.dev\.' | grep -v '\.profile\.')
for mod in expo-audio expo-location expo-video react-native-kb @gorhom/bottom-sheet lottie-react-native react-native-safe-area-context; do
  hits=$(echo "$PROD" | xargs g
```

</details>
