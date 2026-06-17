---
name: zhixianio__botdrop-android
source: https://github.com/zhixianio/botdrop-android/blob/c774a84b1f8442cfd384083dc3cfffa144b1de50/CLAUDE.md
repo: zhixianio/botdrop-android
kind: claude-md
stars: 388
last_pushed: 2026-03-18T07:23:54Z
license: gpl-3.0
score: 8
domains: [android-development, java-gradle]
tags: [environment-setup, troubleshooting, build-scripts]
curated: 2026-06-15
curated_by: config-scout
---

# zhixianio/botdrop-android — claude-md

**Why it's worth keeping:** The 'Common Issues' section is excellent; it preemptively solves specific environmental failures (like SSL or IPv6 networking issues) that would otherwise cause an AI agent to loop on errors. It also explicitly handles the JAVA_HOME export pattern required for Gradle success.

**Summary:** Provides precise environment variable configurations for JDK and granular build/troubleshooting commands.

**Source credibility:** Active repository with recent updates and reasonable star count indicating a real-world project.

**Recency:** Extremely current, including future-dated troubleshooting entries from February 2026.

**Source:** [zhixianio/botdrop-android/CLAUDE.md](https://github.com/zhixianio/botdrop-android/blob/c774a84b1f8442cfd384083dc3cfffa144b1de50/CLAUDE.md) · 388★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Code Development Guide

This file contains project-specific context for AI assistants working on this codebase.

## Local Development Environment

### Java/JDK Configuration

**This machine uses Homebrew-installed OpenJDK 17:**
```bash
# Java location
JAVA_HOME=/opt/homebrew/opt/openjdk@17
PATH="$JAVA_HOME/bin:$PATH"

# Version
OpenJDK 17.0.18

# Installation path
/opt/homebrew/opt/openjdk@17 -> /opt/homebrew/Cellar/openjdk@17/17.0.18
```

**For Gradle builds, set environment:**
```bash
export JAVA_HOME=/opt/homebrew/opt/openjdk@17
export PATH="$JAVA_HOME/bin:$PATH"
```

**Verify Java:**
```bash
$JAVA_HOME/bin/java -version
# Should output: openjdk version "17.0.18"
```

### Building the Project

**Debug APK:**
```bash
export JAVA_HOME=/opt/homebrew/opt/openjdk@17
./gradlew clean assembleDebug

# Output: app/build/outputs/apk/debug/botdrop-app_*_debug.apk
```

**Run tests:**
```bash
export JAVA_HOME=/opt/homebrew/opt/openjdk@17
./gradlew :app:testDebugUnitTest
```

**Clean build:**
```bash
export JAVA_HOME=/opt/homebrew/opt/openjdk@17
./gradlew clean
```

## Project Structure

- **Android App:** `app/` - Main BotDrop Android application
- **Termux Core:** `termux-shared/`,
```

</details>
