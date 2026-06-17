---
name: yahiafarghaly__PrettyOS
source: https://github.com/yahiafarghaly/PrettyOS/blob/d2c8370011475b78c8037eaa3c1ac8516be2d9b2/CLAUDE.md
repo: yahiafarghaly/PrettyOS
kind: claude-md
stars: 53
last_pushed: 2026-05-23T11:03:38Z
license: mit
score: 9
domains: [embedded, systems-programming]
tags: [rtos, c, low-level]
curated: 2026-06-15
curated_by: config-scout
---

# yahiafarghaly/PrettyOS — claude-md

**Why it's worth keeping:** The inclusion of explicit compilation patterns for different architectures and a comprehensive list of configuration macros allows Claude to perform builds and system tuning without ambiguity.

**Summary:** Provides highly specific build commands for multiple targets and a detailed structural map of the kernel architecture.

**Source credibility:** A decent star count (53) and recent activity indicate a legitimate, well-maintained niche project.

**Recency:** Very current; the content is relevant to modern embedded toolchains.

**Source:** [yahiafarghaly/PrettyOS/CLAUDE.md](https://github.com/yahiafarghaly/PrettyOS/blob/d2c8370011475b78c8037eaa3c1ac8516be2d9b2/CLAUDE.md) · 53★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

PrettyOS is a preemptive hard real-time kernel (RTOS) for embedded devices. It's written in C with minimal assembly for context switching. The kernel supports two scheduling modes: Static Priority (RMS - Rate Monotonic Scheduling) and EDF (Earliest Deadline First).

## Build System

There is no Makefile or CMake. Projects are built by integrating kernel source files with port-specific files and compiling with the appropriate toolchain.

**For POSIX/Linux development:**
```bash
# Compile an application (example pattern)
gcc -I kernel/ -I port/posix/cpu/GNU/ -I port/posix/bsp/ -I Applications/ \
    kernel/*.c port/posix/cpu/GNU/*.c port/posix/bsp/*.c your_app.c \
    -lpthread -lrt -o your_app

# POSIX port requires real-time priority configuration:
# Add to /etc/security/limits.conf: "username - rtprio unlimited"
```

**For ARM Cortex-M4 (TI LM4F120):**
- Use embedded toolchain (arm-none-eabi-gcc)
- Link with `port/arm/cortex-m4/bsp/ek-lm4f120xl/ek-lm4f120xl.lds`
- Include startup file from BSP directory

## Architecture

```
kernel/
```

</details>
