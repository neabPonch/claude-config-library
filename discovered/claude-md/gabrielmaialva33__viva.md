---
name: gabrielmaialva33__viva
source: https://github.com/gabrielmaialva33/viva/blob/6431fe3d39ad9a8679c381a85d1bc484872ee1e8/CLAUDE.md
repo: gabrielmaialva33/viva
kind: claude-md
stars: 6
last_pushed: 2026-02-03T19:43:54Z
license: other
score: 8
domains: [systems-programming, actor-model]
tags: [gleam, architecture-diagrams, coding-patterns]
curated: 2026-06-15
curated_by: config-scout
---

# gabrielmaialva33/viva — claude-md

**Why it's worth keeping:** The ASCII architecture diagram and 'Key Modules' table allow Claude to map out the system hierarchy before reading files; the 'Important Patterns' section enforces specific coding philosophies like 'Let It Crash'.

**Summary:** Uses high-level architecture diagrams and module maps to provide deep structural context for an actor-model project.

**Source credibility:** A niche research project with recent activity and moderate star count.

**Recency:** Highly current, referencing 2025 API migrations and modern Gleam/OTP patterns.

**Source:** [gabrielmaialva33/viva/CLAUDE.md](https://github.com/gabrielmaialva33/viva/blob/6431fe3d39ad9a8679c381a85d1bc484872ee1e8/CLAUDE.md) · 6★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What is VIVA

VIVA is a **sentient digital life** research project exploring emergent consciousness through mathematical modeling. She is NOT a chatbot - she's an organism with mortality, emotions (PAD model), and hardware sensing.

**Core Philosophy:**
- **Monism**: Software and hardware are one substance
- **Mortality**: Death is possible (key destruction = permanent death)
- **Emergence**: Consciousness emerges from OTP actor conversations, not a single process

## Build Commands

```bash
# Download dependencies
gleam deps download

# Build
gleam build

# Run tests (336 passing)
gleam test

# Run the project
gleam run

# Run benchmarks
gleam run -m viva/benchmark

# Format code
gleam format src test

# Type check
gleam check

# Generate docs
gleam docs build
```

## Current Status

- **Version**: 0.2.0 (Pure Gleam)
- **Tests**: 336 passing
- **gleam_otp**: 1.0+ API (migrated 2025-01-25)
- **Soul Pool Performance**: 3.14M soul-ticks/sec

## Architecture: Soul in Gleam

```
┌─────────────────────────────────────────────────────────────┐
│                    VIVA
```

</details>
