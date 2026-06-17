---
name: wordpress-mobile__WordPress-Android
source: https://github.com/wordpress-mobile/WordPress-Android/blob/d3b5edc2ad642b9165c12afc0eb4367269bf6f67/CLAUDE.md
repo: wordpress-mobile/WordPress-Android
kind: claude-md
stars: 3140
last_pushed: 2026-06-16T15:52:12Z
license: gpl-2.0
score: 9
domains: [mobile-android, open-source]
tags: [android, gradle, workflow-automation, architecture]
curated: 2026-06-16
curated_by: config-scout
---

# wordpress-mobile/WordPress-Android — claude-md

**Why it's worth keeping:** It utilizes high-value 'negative constraints' (e.g., when NOT to run tools) and includes a mandatory Git Checklist to control agent autonomy. The inclusion of a complex SOP for release notes is an excellent example of providing workflow context.

**Summary:** A comprehensive technical manual that covers build commands, multi-module architecture, and specific coding standards for a large Android project.

**Source credibility:** Highly credible, originating from a major open-source project with high star count and recent activity.

**Recency:** Current; utilizes modern Android standards like Version Catalogs and Jetpack Compose.

**Source:** [wordpress-mobile/WordPress-Android/CLAUDE.md](https://github.com/wordpress-mobile/WordPress-Android/blob/d3b5edc2ad642b9165c12afc0eb4367269bf6f67/CLAUDE.md) · 3140★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Build and Test Commands

### Main Build Commands
- `./gradlew assembleWordPressDebug` - Build debug APK for WordPress app
- `./gradlew assembleJetpackDebug` - Build debug APK for Jetpack app
- `./gradlew installWordPressDebug` - Install debug APK to connected device
- `./gradlew installJetpackDebug` - Install debug APK for Jetpack to device

### Testing Commands
- `./gradlew :WordPress:testWordPressDebugUnitTest` - Run unit tests for WordPress app
- `./gradlew :WordPress:connectedWordPressDebugAndroidTest` - Run instrumented tests for WordPress app
- `bundle exec fastlane build_and_run_instrumented_test app:wordpress` - Build and run WordPress instrumented tests in Firebase Test Lab
- `bundle exec fastlane build_and_run_instrumented_test app:jetpack` - Build and run Jetpack instrumented tests in Firebase Test Lab

### Code Quality Commands
- `./gradlew checkstyle` - Run Checkstyle linter (generates report in `WordPress/build/reports/checkstyle/checkstyle.html`)
- `./gradlew detekt` - Run Detekt linter for Kotlin (generates report in `WordPress/build/reports/detekt
```

</details>
