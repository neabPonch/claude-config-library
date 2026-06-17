---
name: kurikomi-labs__komi-store
source: https://github.com/kurikomi-labs/komi-store/blob/55b51634e5fd4140ec704672c0e672e9c94fe2c1/CLAUDE.md
repo: kurikomi-labs/komi-store
kind: claude-md
stars: 15342
last_pushed: 2026-06-14T17:09:26Z
license: apache-2.0
score: 9
domains: [mobile-app, desktop-app, kotlin-multiplatform]
tags: [kmp, kotlin, architecture, mvvm, compose]
curated: 2026-06-15
curated_by: config-scout
---

# kurikomi-labs/komi-store — claude-md

**Why it's worth keeping:** The inclusion of an explicit 'State pattern' code snippet and a step-by-step 'Adding a feature' procedure is perfect for guiding LLM-based development. It also documents high-complexity logic like the OAuth handoff and bit-packed ID encoding, which prevents hallucination in sensitive areas.

**Summary:** A highly detailed technical specification for a Kotlin Multiplatform project covering architecture, build processes, and complex platform-specific logic. It provides explicit patterns for state management, dependency injection, and feature implementation.

**Source credibility:** High; highly starred (15k+) active open-source project with recent maintenance.

**Recency:** Current; includes modern versions of Kotlin, Compose, and Ktor libraries.

**Source:** [kurikomi-labs/komi-store/CLAUDE.md](https://github.com/kurikomi-labs/komi-store/blob/55b51634e5fd4140ec704672c0e672e9c94fe2c1/CLAUDE.md) · 15342★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Komi Store

Cross-platform app store for GitHub + Codeberg + Forgejo releases. **Kotlin Multiplatform** + **Compose Multiplatform**. Android (min API 26) + Desktop (JVM: Win/macOS/Linux). Package `zed.rainxch.githubstore`. Version 1.8.3 (code 18). Target SDK 36.

## Build

```bash
./gradlew :composeApp:assembleDebug                                    # Android
./gradlew :composeApp:run                                              # Desktop dev
./gradlew :composeApp:packageExe :composeApp:packageMsi                # Win installer
./gradlew :composeApp:packageDmg :composeApp:packagePkg                # macOS
./gradlew :composeApp:packageDeb :composeApp:packageRpm                # Linux
./gradlew build                                                        # full
```

JDK 21+. Android SDK for Android.

## Structure

```
composeApp/            # entry points, navigation, DI wiring (commonMain / androidMain / jvmMain)
core/
  domain/              # interfaces, models, use cases (no framework deps)
  data/                # repos, Ktor, Room, Koin, platform impls
  presentation/        # Material 3 theme + reusable components + 13-locale strings
feature/
  apps auth details dev-profile
```

</details>
