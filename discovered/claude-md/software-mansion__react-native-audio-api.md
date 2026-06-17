---
name: software-mansion__react-native-audio-api
source: https://github.com/software-mansion/react-native-audio-api/blob/9d713823986279611a4a1886220a88118e78d2a8/CLAUDE.md
repo: software-mansion/react-native-audio-api
kind: claude-md
stars: 785
last_pushed: 2026-06-12T12:31:06Z
license: mit
score: 10
domains: [mobile-development, systems-programming, cross-platform]
tags: [architecture-driven, agent-orchestration, self-documenting]
curated: 2026-06-15
curated_by: config-scout
---

# software-mansion/react-native-audio-api — claude-md

**Why it's worth keeping:** Uses 'Golden Reference' mapping to ensure pattern consistency, includes specific subagent parallelization instructions, and defines a self-healing loop for documentation maintenance.

**Summary:** Provides a deep architectural breakdown of a complex cross-platform audio engine and establishes a sophisticated, self-maintaining 'Skills' ecosystem for agentic work.

**Source credibility:** High; maintained by Software Mansion with significant community traction (785 stars).

**Recency:** Extremely current; specifically optimized for Claude Code's agentic behaviors like subagents and skill files.

**Source:** [software-mansion/react-native-audio-api/CLAUDE.md](https://github.com/software-mansion/react-native-audio-api/blob/9d713823986279611a4a1886220a88118e78d2a8/CLAUDE.md) · 785★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

`react-native-audio-api` is a high-performance Web Audio API-compatible audio engine for React Native, maintained by Software Mansion. It provides audio playback, recording, DSP processing, and real-time analysis across iOS, Android, and Web.

## Architecture

### Monorepo Structure
```
packages/react-native-audio-api/   # Main library
apps/common-app/                   # Example RN app
apps/fabric-example/               # New Architecture example app
packages/audiodocs/                # Documentation
packages/custom-node-generator/    # Code generation tooling
```

### Layers (from JS to hardware)

1. **TypeScript API** (`src/`) — node implementations (`src/core/`), browser passthrough (`src/web-core/`), platform system APIs (`src/system/`), TurboModule specs (`src/specs/`), hooks, events, utils
2. **C++ Engine** (`common/cpp/audioapi/`) — node engine (`core/`), SIMD DSP (`dsp/`), JSI HostObjects, audio events, prebuilt external libraries (`external/`)
3. **Android Native** (`android/`) — CMake + Gradle, Kotlin module, C++ JNI glue (`src/main
```

</details>
