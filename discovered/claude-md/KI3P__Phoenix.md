---
name: KI3P__Phoenix
source: https://github.com/KI3P/Phoenix/blob/e58ff10ea18e76585ce4c7a16f1e3c44374f85ff/CLAUDE.md
repo: KI3P/Phoenix
kind: claude-md
stars: 12
last_pushed: 2026-06-08T10:54:40Z
license: gpl-3.0
score: 9
domains: [embedded, firmware]
tags: [sdr, state-machines, real-time, cpp]
curated: 2026-06-15
curated_by: config-scout
---

# KI3P/Phoenix — claude-md

**Why it's worth keeping:** It defines vital runtime limits (the 10ms loop rule) and mandatory behavioral patterns (state machine usage), preventing the AI from introducing timing violations or bypassing control logic.

**Summary:** Provides highly specific architectural blueprints, directory mapping, and critical real-time constraints for an embedded C++ project.

**Source credibility:** High-quality documentation for a specialized hardware/firmware project.

**Recency:** Current; includes up-to-date toolchain versions and modern build workflows.

**Source:** [KI3P/Phoenix/CLAUDE.md](https://github.com/KI3P/Phoenix/blob/e58ff10ea18e76585ce4c7a16f1e3c44374f85ff/CLAUDE.md) · 12★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md - Phoenix SDR Radio Project

## Project Overview

This is the **Phoenix SDR (Software Defined Radio)** project - firmware for a Teensy 4.1-based amateur radio transceiver. The project implements a complete SDR radio system using state machines for hardware control and real-time digital signal processing.

## Architecture

### Core Components
- **Hardware Platform**: Teensy 4.1 microcontroller
- **Language**: C/C++ with Arduino framework (`.ino`, `.cpp`, `.h` files)
- **State Machines**: Generated from UML diagrams using StateSmith
- **Real-time DSP**: OpenAudio library for signal processing
- **Testing**: Google Test framework with comprehensive unit tests

### Key Features
- Dual VFO (Variable Frequency Oscillator) operation
- SSB (Single Sideband) and CW (Morse Code) modes
- Real-time digital signal processing
- State machine-controlled hardware management
- CAT (Computer Aided Transceiver) control interface
- Comprehensive test coverage with mocking framework

## Code Structure

### Main Source Directory: `code/src/PhoenixSketch/`
- **PhoenixSketch.ino**: Main Arduino sketch entry point
- **Loop.cpp/h**: Main program loop implementation
- **ModeSm.cpp/h**: Radio mode
```

</details>
