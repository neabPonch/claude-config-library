---
name: wentbackward__nv-monitor
source: https://github.com/wentbackward/nv-monitor/blob/ae1f4261d8172d9f8a44a49684bb889cdac701c7/CLAUDE.md
repo: wentbackward/nv-monitor
kind: claude-md
stars: 289
last_pushed: 2026-05-07T11:58:37Z
license: mit
score: 9
domains: [cli-tools, systems-programming]
tags: [c, linux, performance, hardware-interfacing]
curated: 2026-06-15
curated_by: config-scout
---

# wentbackward/nv-monitor — claude-md

**Why it's worth keeping:** Uses high-stakes warnings to prevent memory growth and locale bugs; explains the 'why' behind specific code logic to prevent improper AI refactoring.

**Summary:** Provides deep system architecture details and critical engineering constraints for a low-level C monitoring tool.

**Source credibility:** Highly credible repository focused on specialized NVIDIA hardware with recent activity.

**Recency:** Extremely current, referencing latest Blackwell/GB20 architectures.

**Source:** [wentbackward/nv-monitor/CLAUDE.md](https://github.com/wentbackward/nv-monitor/blob/ae1f4261d8172d9f8a44a49684bb889cdac701c7/CLAUDE.md) · 289★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

nv-monitor is a single-file C terminal system monitor for the NVIDIA DGX Spark (Grace ARM CPU + GB10 Blackwell GPU). It combines CPU, memory, and GPU monitoring in one ncurses TUI.

## Build

```bash
make          # builds nv-monitor binary (-O3 -march=native)
make portable # builds without -march=native (for CI/distribution)
make test     # builds and runs unit tests
make clean    # removes binaries
```

Direct compilation: `gcc -O2 -Wall -Wextra -std=gnu11 -o nv-monitor nv-monitor.c -lncursesw -ldl -lpthread`

Dependencies: `build-essential`, `libncurses-dev`

Works on both **aarch64** (DGX Spark) and **x86_64**. On x86, ARM core type labels are omitted; everything else works identically.

## Architecture

Everything is in `nv-monitor.c` (~1640 lines). Key sections:

- **NVML dynamic loading** (line ~115): Loads `libnvidia-ml.so.1` via `dlopen`/`dlsym` at runtime. Uses a variadic LOAD macro to try versioned symbols first (e.g. `nvmlInit_v2` before `nvmlInit`). All NVML function pointers are prefixed with `p` (e.g. `pNvmlInit`).
- **CPU sampling**: Reads
```

</details>
