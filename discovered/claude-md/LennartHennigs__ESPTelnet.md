---
name: LennartHennigs__ESPTelnet
source: https://github.com/LennartHennigs/ESPTelnet/blob/27de3ca875df74ac8f123071de61d7d0a0d6724b/CLAUDE.md
repo: LennartHennigs/ESPTelnet
kind: claude-md
stars: 256
last_pushed: 2026-05-09T17:05:11Z
license: mit
score: 9
domains: [embedded-systems, firmware]
tags: [arduino, esp32, platformio, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# LennartHennigs/ESPTelnet — claude-md

**Why it's worth keeping:** Exemplifies the use of 'ownership' descriptions (defining which class manages specific state) and explicit design constraints that prevent logic errors during code generation.

**Summary:** Provides a comprehensive architectural map of class hierarchies and specific PlatformIO build commands for multiple environments.

**Source credibility:** Strong; 256 stars indicates a well-established, community-vetted library.

**Recency:** Very current; provides the exact technical depth required by modern AI coding agents.

**Source:** [LennartHennigs/ESPTelnet/CLAUDE.md](https://github.com/LennartHennigs/ESPTelnet/blob/27de3ca875df74ac8f123071de61d7d0a0d6724b/CLAUDE.md) · 256★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

ESPTelnet is an Arduino library (v2.2.3) for ESP8266/ESP32 that sets up a single-client telnet server. It's primarily used to send debug/status output to a remote terminal when no Serial connection is available.

## Build Commands (PlatformIO)

```bash
# Build for default environment (d1_mini_lite)
pio run

# Build for a specific board
pio run -e <environment_name>
# e.g.: pio run -e esp32dev
#       pio run -e m5stack-core-esp32
#       pio run -e arduino_nano_esp32

# List all available environments: d1_mini_lite, d1_mini, nodemcuv2, esp12e,
# esp32dev, m5stack-core-esp32, m5stack-fire, m5stick-c, arduino_nano_esp32,
# esp32-s2-saola-1, esp32-c3-devkitm-1
```

There is no automated test suite — validation is done by building against real hardware environments.

## Architecture

The library has a three-class hierarchy in `src/`:

```
ESPTelnetBase (ESPTelnetBase.h / .cpp)
  ├── ESPTelnet (ESPTelnet.h / .cpp)         — print/println/printf + line-mode input
  └── ESPTelnetStream (ESPTelnetStream.h / .cpp) — Arduino Stream interface
```

**`ESPTel
```

</details>
