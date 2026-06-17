---
name: OpenAstroTech__OpenAstroTracker-Firmware
source: https://github.com/OpenAstroTech/OpenAstroTracker-Firmware/blob/9d418ed54ed3dee43bd8dd41c9c9e1ab9ba2d806/CLAUDE.md
repo: OpenAstroTech/OpenAstroTracker-Firmware
kind: claude-md
stars: 111
last_pushed: 2026-05-28T15:57:37Z
license: mit
score: 9
domains: [embedded-c++, firmware]
tags: [platformio, arduino, hardware-abstraction]
curated: 2026-06-16
curated_by: config-scout
---

# OpenAstroTech/OpenAstroTracker-Firmware — claude-md

**Why it's worth keeping:** The explicit explanation of configuration precedence (local vs. advanced vs. constants) prevents the AI from making incorrect assumptions about user settings, while the platform-specific execution details (AVR interrupts vs. ESP32 tasks) are critical for correctness.

**Summary:** Provides highly specific PlatformIO build/test commands and explains a complex, multi-layered hardware configuration hierarchy.

**Source credibility:** Strong; an active open-source hardware project with significant community interest.

**Recency:** Very current; uses modern build toolchains and developer workflows.

**Source:** [OpenAstroTech/OpenAstroTracker-Firmware/CLAUDE.md](https://github.com/OpenAstroTech/OpenAstroTracker-Firmware/blob/9d418ed54ed3dee43bd8dd41c9c9e1ab9ba2d806/CLAUDE.md) · 111★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

OpenAstroTracker-Firmware is embedded C++ firmware for the OpenAstroTracker automated astronomy mount. It supports multiple hardware platforms (AVR ATmega2560 and ESP32) with various stepper motor drivers, display types, and accessories.

## Build System

PlatformIO is the build system. The project uses the Arduino framework.

### Common Commands

```shell
# Build for a specific board environment
pio run -e ramps
pio run -e esp32
pio run -e mksgenlv21
pio run -e mksgenlv2
pio run -e mksgenlv1
pio run -e oaeboardv1

# Upload firmware
pio run -e ramps -t upload

# Run unit tests (native platform)
pio test -e native

# Run unit tests with coverage report (requires gcovr: pip install gcovr)
./scripts/test-coverage.sh          # defaults to -e native
./scripts/test-coverage.sh -e native
# Report: .pio/build/native/coverage_report/index.html

# Run matrix build (tests many configuration combinations across boards)
python matrix_build.py -b ramps     # single board
python matrix_build.py              # all boards

# Format code (clang-format v12 require
```

</details>
