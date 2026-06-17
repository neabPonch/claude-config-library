---
name: mybigday__whisper.rn
source: https://github.com/mybigday/whisper.rn/blob/eadd9cdd25ba84d49ba363e95a204de804e06529/CLAUDE.md
repo: mybigday/whisper.rn
kind: claude-md
stars: 789
last_pushed: 2026-06-02T05:53:22Z
license: mit
score: 9
domains: [mobile-development, cross-platform, audio-processing]
tags: [react-native, cpp, jsi, performance]
curated: 2026-06-15
curated_by: config-scout
---

# mybigday/whisper.rn — claude-md

**Why it's worth keeping:** The multi-layer architecture breakdown and specific low-level technical constraints (audio specs, memory management) are vital to prevent AI hallucinations during native integration tasks.

**Summary:** Provides comprehensive architectural mapping for a complex C++/JavaScript bridge and detailed development workflows.

**Source credibility:** Highly credible; significant star count and active maintenance recorded in the last month.

**Recency:** Very current with modern React Native, TurboModules, and JSI patterns.

**Source:** [mybigday/whisper.rn/CLAUDE.md](https://github.com/mybigday/whisper.rn/blob/eadd9cdd25ba84d49ba363e95a204de804e06529/CLAUDE.md) · 789★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# whisper.rn - Development Guidelines

## Project Overview

whisper.rn is a React Native binding for [whisper.cpp](https://github.com/ggerganov/whisper.cpp), enabling high-performance inference of OpenAI's Whisper automatic speech recognition (ASR) model on iOS and Android devices.

**Key Features:**
- Native speech-to-text transcription via whisper.cpp
- Voice Activity Detection (VAD) using Silero VAD model
- Realtime transcription with auto-slicing and memory management
- Core ML support for iOS (encoder acceleration)
- Metal/GPU acceleration support
- JSI (JavaScript Interface) bindings for efficient ArrayBuffer transfers

## General

- Pay attention to code readability.
- Add comments appropriately, no need to explain the obvious.
- Apply first-principles thinking when appropriate.

## Development Commands

### Setup and Bootstrap
```bash
yarn                    # Install dependencies
yarn bootstrap          # Setup project (install deps + build whisper.cpp submodule)
```

### Code Quality
```bash
yarn typecheck          # Type-check TypeScript files
yarn lint               # Lint files with ESLint
yarn lint --fix         # Fix lint errors
yarn test               # Run Jest uni
```

</details>
