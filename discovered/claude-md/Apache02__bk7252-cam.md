---
name: Apache02__bk7252-cam
source: https://github.com/Apache02/bk7252-cam/blob/33ef5eb8eed969dc89c37c3a3b656a632d40747f/CLAUDE.md
repo: Apache02/bk7252-cam
kind: claude-md
stars: 5
last_pushed: 2026-06-14T19:54:23Z
license: unknown
score: 9
domains: [embedded-systems, firmware, c]
tags: [arm, freertos, cmake, hardware-interfacing]
curated: 2026-06-15
curated_by: config-scout
---

# Apache02/bk7252-cam — claude-md

**Why it's worth keeping:** Includes specific 'gotchas' like printf limitations and CRC wrapping requirements; provides a clear mental model of the layered architecture to help AI navigate dependencies.

**Summary:** A highly detailed technical manual for a bare-metal embedded project that maps the complex CMake hierarchy and hardware interaction layers.

**Source credibility:** High: popular repository (5 stars) with very recent activity.

**Recency:** Very current, including instructions tailored for Claude Code's specialized skills.

**Source:** [Apache02/bk7252-cam/CLAUDE.md](https://github.com/Apache02/bk7252-cam/blob/33ef5eb8eed969dc89c37c3a3b656a632d40747f/CLAUDE.md) · 5★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

Bare-metal / FreeRTOS firmware for a BK7252-based A9 camera (ARM968E-S, thumb-interwork). Cross-compiled with `arm-none-eabi-gcc` (C11 / C++20, `-O2`, `--specs=nano.specs`, `-fno-exceptions`).

## Build

CMake out-of-tree build. The board must be selected (defaults to `A9_B_V1_3`):

```sh
mkdir -p build
(cd build && cmake -DBOARD=A9_B_V1_3 .. && make freertos_shell)
```

Other application targets (see `src/applications/`): `hello`, `blink`, `shell`, `freertos_example`, `freertos_shell`, `ram_loader`. Standalone driver/peripheral tests live under `src/tests/` (currently `test_gdma`, `test_random`, `test_security`) — they are separate IRAM firmware images, not a unit-test harness.

`src/CMakeLists.txt` auto-globs both `applications/` and `tests/` — dropping a new subdirectory with its own `CMakeLists.txt` into either is enough to register it as a target.

Each firmware target produced by `bk_firmware()` (see `cmake/firmware.cmake`) post-processes the ELF into `<target>.bin` and a CRC-wrapped `<target>_crc.bin`, copying the latter to `build/app_crc.bin`. Tar
```

</details>
