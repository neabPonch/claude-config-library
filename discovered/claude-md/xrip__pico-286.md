---
name: xrip__pico-286
source: https://github.com/xrip/pico-286/blob/2ba88bf17de8e69c86f9256e22a241e8d31e8c96/CLAUDE.md
repo: xrip/pico-286
kind: claude-md
stars: 291
last_pushed: 2026-03-04T16:32:15Z
license: mit
score: 9
domains: [embedded-systems, emulation, c]
tags: [cmake, low-level, architecture-mapping, ai-personas]
curated: 2026-06-15
curated_by: config-scout
---

# xrip/pico-286 — claude-md

**Why it's worth keeping:** Provides exact, copy-pasteable CMake commands with mutually exclusive flags to prevent build errors; maps file organization directly to system components; implements an 'AI Team Configuration' for task-specific guidance.

**Summary:** A high-density technical guide covering complex build constraints, hardware abstraction layers, and multi-platform architecture. It includes a unique persona mapping strategy to direct AI focus for specialized tasks.

**Source credibility:** High (291 stars, active maintenance)

**Recency:** Current and highly optimized for modern Claude Code workflows

**Source:** [xrip/pico-286/CLAUDE.md](https://github.com/xrip/pico-286/blob/2ba88bf17de8e69c86f9256e22a241e8d31e8c96/CLAUDE.md) · 291★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Pico-286 is a PC emulator targeting Intel 8086/8088/80186/286 CPUs, designed to run on Raspberry Pi Pico (RP2040/RP2350) microcontrollers. The project emulates classic PC hardware including various graphics cards (CGA, TGA, EGA, VGA), sound cards (PC Speaker, Adlib, Sound Blaster, MPU-401), and peripherals.

## Build System

The project uses CMake with two main build targets:

### Cross-platform builds:
- **Host build (Windows/Linux)**: `cmake -DCMAKE_BUILD_TYPE=Release -DPICO_PLATFORM=host`
- **Pico RP2040**: `cmake -DCMAKE_BUILD_TYPE=Release -DPICO_PLATFORM=rp2040`  
- **Pico RP2350**: `cmake -DCMAKE_BUILD_TYPE=Release -DPICO_PLATFORM=rp2350`

### Essential build options:
All builds require exactly one display and one audio option:

**Display options (mutually exclusive):**
- `-DENABLE_TFT=ON` - TFT display via ST7789
- `-DENABLE_VGA=ON` - VGA output
- `-DENABLE_HDMI=ON` - HDMI output (forces CPU to 378MHz)

**Audio options (mutually exclusive):**
- `-DENABLE_I2S_SOUND=ON` - I2S audio output
- `-DENABLE_PWM_SOUND=ON` - PWM audio output  
- `-DE
```

</details>
