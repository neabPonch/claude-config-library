---
name: Shopify__flash-list__skill
source: https://github.com/Shopify/flash-list/blob/20e29c20e440a0a8e0492c303c254dbefee3ad62/.claude/skills/upgrade-react-native/SKILL.md
repo: Shopify/flash-list
kind: skill
stars: 7114
last_pushed: 2026-06-13T02:39:59Z
license: mit
score: 9
domains: [mobile-development, react-native, devops]
tags: [upgrade-procedure, android, ios, build-systems]
curated: 2026-06-15
curated_by: config-scout
---

# Shopify/flash-list — skill

**Why it's worth keeping:** Uses the 'rn-diff-purge' technique to establish ground truth; offers high-value patterns for complex file changes like MainApplication.kt and Metro config transitions.

**Summary:** Provides a highly detailed technical SOP for upgrading React Native versions across JS, Android, and iOS environments. It includes specific instructions for build tool configuration, dependency management, and verification.

**Source credibility:** High; comes from Shopify's official FlashList repository, a mission-critical library.

**Recency:** Highly current, referencing recent React Native versions (0.79/0.84) and modern architectural patterns.

**Source:** [Shopify/flash-list/.claude/skills/upgrade-react-native/SKILL.md](https://github.com/Shopify/flash-list/blob/20e29c20e440a0a8e0492c303c254dbefee3ad62/.claude/skills/upgrade-react-native/SKILL.md) · 7114★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: upgrade-react-native
description: Upgrade the React Native fixture app to a new version. Covers JS deps, Android (Gradle, Kotlin, SDK), iOS (Podfile, pbxproj), Metro config, and third-party libraries.
---

# Upgrade React Native Fixture App

## Overview

The fixture app lives in `fixture/react-native/`. It is the primary test vehicle for FlashList on iOS and Android. The web fixture (`fixture/web/`) uses Expo and is independent — check it builds after the upgrade but it does not need the same dependency changes.

## Step 1 — Research the Target Version

1. Check the latest stable RN version:
   ```bash
   npm view react-native@latest version
   ```

2. Use the **rn-diff-purge** repo to see the exact template diff between your current and target version:
   ```
   https://raw.githubusercontent.com/react-native-community/rn-diff-purge/release/<version>/RnDiffApp/<file>
   ```
   Key files to fetch:
   - `package.json` — React version, CLI versions, dev dep versions
   - `android/build.gradle` — SDK versions, Kotlin version
   - `android/app/build.gradle` — plugin names, dependency patterns
   - `android/gradle.properties` — feature flags (newArch, hermes, edgeToEdge)
   - `
```

</details>
