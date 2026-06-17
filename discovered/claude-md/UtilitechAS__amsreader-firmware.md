---
name: UtilitechAS__amsreader-firmware
source: https://github.com/UtilitechAS/amsreader-firmware/blob/a88a0beb9c57b33bf9417522a894958f300e45e3/CLAUDE.md
repo: UtilitechAS/amsreader-firmware
kind: claude-md
stars: 461
last_pushed: 2026-06-12T20:22:06Z
license: other
score: 9
domains: [embedded-systems, iot, firmware]
tags: [platformio, esp32, architecture, build-instructions]
curated: 2026-06-15
curated_by: config-scout
---

# UtilitechAS/amsreader-firmware — claude-md

**Why it's worth keeping:** It includes critical 'gotchas' regarding platform abstraction (Arduino vs. Native), detailed translation workflows, and explicit instructions on how to handle configuration overrides.

**Summary:** A highly structured guide that provides deep architectural context, including data flow diagrams and specific build-order dependencies like UI compilation requirements.

**Source credibility:** Strong; high star count and very recent activity indicates a well-maintained, real-world production codebase.

**Recency:** Current; provides specific modern environment requirements for Node.js and Python tools.

**Source:** [UtilitechAS/amsreader-firmware/CLAUDE.md](https://github.com/UtilitechAS/amsreader-firmware/blob/a88a0beb9c57b33bf9417522a894958f300e45e3/CLAUDE.md) · 461★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

AMS Reader (`ams2mqtt`) is PlatformIO/Arduino firmware for ESP8266 and ESP32 devices that reads data from European IEC-62056 compliant smart electricity meters via M-Bus/HAN port, decodes it, and publishes to MQTT. It also serves a Svelte SPA web interface.

## Prerequisites

- Python 3.9+ with `platformio` and `css_html_js_minify` (`pip install -U platformio css_html_js_minify`)
- Node.js 19.x (for Svelte UI)

## Setup (first time)

```bash
# Required: copy and customize local build config
cp platformio-user.ini-example platformio-user.ini

# Build Svelte frontend FIRST (must exist before firmware build)
cd ui && npm ci && npm run build && cd -

# Install PlatformIO library dependencies
pio pkg install
```

## Build Commands

```bash
pio run -e esp32s2            # Build for a specific target (esp8266, esp32, esp32s2, esp32s3, esp32c3, esp32solo)
pio run                       # Build all envs defined in platformio-user.ini default_envs
pio run -e esp32s2 -t upload  # Build and flash to connected device
pio device monitor            # Serial moni
```

</details>
