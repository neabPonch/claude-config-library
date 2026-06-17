---
name: francescobianco__btproxy.old
source: https://github.com/francescobianco/btproxy.old/blob/bf293a2c92fd542713f838b2672d78c32f189ad5/CLAUDE.md
repo: francescobianco/btproxy.old
kind: claude-md
stars: 1
last_pushed: 2025-10-17T15:46:55Z
license: mit
score: 7
domains: [mobile-android, iot, api]
tags: [android, kotlin, ble, api-spec]
curated: 2026-06-16
curated_by: config-scout
---

# francescobianco/btproxy.old — claude-md

**Why it's worth keeping:** Excellent inclusion of specific shell commands (build/install) and clear documentation of API endpoints with expected data formats (Hex vs JSON).

**Summary:** Provides critical command-line instructions for building/deploying via Gradle/ADB and a detailed API specification for testing the service.

**Source credibility:** Low star count, likely an individual developer project.

**Recency:** Current; follows modern Android development patterns.

**Source:** [francescobianco/btproxy.old/CLAUDE.md](https://github.com/francescobianco/btproxy.old/blob/bf293a2c92fd542713f838b2672d78c32f189ad5/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is **btproxy** - a Bluetooth Low Energy (BLE) proxy project designed to bridge communication between devices and BLE peripherals. The project is currently in planning phase, with comprehensive documentation in Italian describing the intended Android Kotlin implementation.

## Architecture Plan

Based on the NOTES.md documentation, this project will implement:

- **Android Kotlin Application**: Minimal command-line buildable Android app
- **BLE Service**: Foreground service for continuous BLE operations
- **Intent Bridge**: Integration with MacroDroid/Tasker for automation
- **Gradle Build System**: Command-line compilation without Android Studio

### Planned Project Structure
```
btproxy/
├─ build.gradle.kts           # Root build configuration
├─ settings.gradle.kts        # Gradle settings
├─ app/
│  ├─ build.gradle.kts        # App module build config
│  ├─ src/main/AndroidManifest.xml
│  ├─ src/main/java/com/example/bleproxy/
│  │   ├─ MainActivity.kt     # Launch activity
│  │   └─ BleService.kt       # Core BLE proxy service
```

## De
```

</details>
