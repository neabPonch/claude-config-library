---
name: rusefi__rusefi
source: https://github.com/rusefi/rusefi/blob/7bdf409039ac04694d41a6f4f48b4348e7e1c014/CLAUDE.md
repo: rusefi/rusefi
kind: claude-md
stars: 1085
last_pushed: 2026-06-14T21:51:18Z
license: other
score: 9
domains: [embedded, systems-programming, firmware]
tags: [build-system, testing, architecture, embedded]
curated: 2026-06-14
curated_by: config-scout
---

# rusefi/rusefi — claude-md

**Why it's worth keeping:** The 'Deep Dive AI Guidance' pattern—linking to specialized docs for core subsystems—is highly transferable. Additionally, providing specific instructions on how to debug test failures (using logs instead of printf) is an elite-level instruction for an AI agent.

**Summary:** A high-quality guide providing specific build workflows, debugging protocols for unit tests, and a unique 'Deep Dive AI Guidance' section. It bridges the gap between general project info and deep technical domain knowledge.

**Source credibility:** High; a popular (1k+ stars), actively maintained open-source embedded project.

**Recency:** Current; references modern C++ standards and advanced build/test workflows compatible with current AI tools.

**Source:** [rusefi/rusefi/CLAUDE.md](https://github.com/rusefi/rusefi/blob/7bdf409039ac04694d41a6f4f48b4348e7e1c014/CLAUDE.md) · 1085★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

rusEFI is an open-source engine control unit firmware for STM32 microcontrollers.

## Build Commands

Default to building with 12 threads unless otherwise specified (-j12 etc).

### Building Firmware

Each board+chip combination has its own compile script in `firmware/config/boards/<board>/`:

```bash
# Example: Build for Proteus F7
cd firmware/config/boards/proteus
./compile_proteus_f7.sh
```

Outputs are placed in `firmware/deliver/`:
- `rusefi.bin` - Complete image (bootloader + firmware) for blank ECUs
- `rusefi_update.srec` - Update image for bootloader flashing

### Unit Tests

```bash
cd unit_tests
./test.sh

# Run a specific test
./test.sh TestName
```

`test.sh` is the recommended way to run tests as it automatically handles both the build (`make`) and execution.

#### Code Coverage
Coverage reports are generated using `gcovr` (requires Python 3).

```bash
cd unit_tests
./run_coverage.sh
```

This script:
1. Sets up a local Python virtual environment in `unit_tests/venv/`
2. Installs `gcovr`
3. Builds tests with `COVERAGE=yes`
4. Runs al
```

</details>
