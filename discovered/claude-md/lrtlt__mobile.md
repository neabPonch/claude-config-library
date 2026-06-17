---
name: lrtlt__mobile
source: https://github.com/lrtlt/mobile/blob/10d562dc0a9ae2ab2ed0e4e0eee27f9fbed6bfbc/CLAUDE.md
repo: lrtlt/mobile
kind: claude-md
stars: 23
last_pushed: 2026-06-10T21:28:20Z
license: bsd-3-clause
score: 9
domains: [mobile-app, react-native]
tags: [zustand, react-query, ios, android, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# lrtlt/mobile — claude-md

**Why it's worth keeping:** It includes highly specific cross-platform versioning math and clear documentation of the Zustand/MMKV persistence strategy which prevents common state management errors.

**Summary:** A comprehensive technical manual for a React Native app that covers complex build processes and deep architectural patterns.

**Source credibility:** High; based on a real-world production mobile application with recent commits.

**Recency:** Current; reflects modern development standards and libraries.

**Source:** [lrtlt/mobile/CLAUDE.md](https://github.com/lrtlt/mobile/blob/10d562dc0a9ae2ab2ed0e4e0eee27f9fbed6bfbc/CLAUDE.md) · 23★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

LRT.lt is a React Native mobile application (iOS and Android) for the Lithuanian public broadcasting service. The app provides access to news articles, live TV/radio streams, podcasts, videos, and weather information.

## Development Commands

### Running the App

```bash
# iOS
yarn run-ios                                    # Build & run in debug mode
react-native run-ios --configuration Release   # Build & run in release mode

# Android
yarn run-android                                # Build & run in debug mode
react-native run-android --variant=release     # Build & run in release mode

# Metro bundler
yarn start                                      # Start the Metro bundler
```

### Clean Build

```bash
# macOS/Linux (includes iOS pod install)
yarn clean-build

# Windows (includes Android gradlew clean)
yarn clean-build-win
```

### Code Quality

```bash
yarn lint          # Run ESLint
yarn ts            # Run TypeScript compiler (skipLibCheck enabled)
yarn test          # Run Jest tests
```

### Platform-specific Setup

**iOS**: After instal
```

</details>
