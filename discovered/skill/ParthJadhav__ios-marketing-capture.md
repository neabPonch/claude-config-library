---
name: ParthJadhav__ios-marketing-capture
source: https://github.com/ParthJadhav/ios-marketing-capture/blob/00ae3cbe2250f6350b66aa23e24ba5883221836c/SKILL.md
repo: ParthJadhav/ios-marketing-capture
kind: skill
stars: 249
last_pushed: 2026-04-10T19:35:01Z
license: mit
score: 9
domains: [ios-development, automation]
tags: [swiftui, screenshots, automation]
curated: 2026-06-14
curated_by: config-scout
---

# ParthJadhav/ios-marketing-capture — skill

**Why it's worth keeping:** The strategy of favoring an in-app launch argument approach over fragile XCUITest/Fastlane setup is highly efficient; the exploration logic for navigating complex SwiftUI state patterns (TabView, NavigationStack) is exceptional.

**Summary:** Automates multi-locale marketing screenshot capture using a DEBUG-only in-app coordinator. It supports both full-screen navigation and isolated component rendering with deterministic data.

**Source credibility:** Strong community validation with 249 stars and recent updates.

**Recency:** Extremely current, incorporating Xcode 16 specific synchronization features.

**Source:** [ParthJadhav/ios-marketing-capture/SKILL.md](https://github.com/ParthJadhav/ios-marketing-capture/blob/00ae3cbe2250f6350b66aa23e24ba5883221836c/SKILL.md) · 249★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: ios-marketing-capture
description: Use when the user wants to automate capture of marketing screenshots for a SwiftUI iOS app across multiple locales, devices, or appearances. Covers full-screen shots, isolated element renders (carousel cards, widgets), and reproducible output naming. Triggers on marketing screenshots, locale screenshots, widget renders, App Store assets, fastlane-alternative, simctl screenshots.
---

# iOS Marketing Capture

## Overview

Automate reproducible marketing screenshot capture for a SwiftUI iOS app across multiple locales, with two parallel output streams:

1. **Full-screen captures** — every marketing-relevant screen, with deterministic seeded data, real status bar / safe-area chrome
2. **Element captures** — isolated renders of specific components (cards, widgets, charts) at any scale, with natural background inside rounded corners and transparency outside

This skill is the **capture** step. If the user also wants Apple-style marketing pages composited around the shots (device mockups, headlines, gradients), combine with the `app-store-screenshots` skill as a post-processing step.

## Core Approach

**In-app capture mode**, not XCUITest. Th
```

</details>
