---
name: djrobson__ReverbWave
source: https://github.com/djrobson/ReverbWave/blob/9349166e83e4455ce64c19d9dfd0363277807597/CLAUDE.md
repo: djrobson/ReverbWave
kind: claude-md
stars: 0
last_pushed: 2026-03-19T01:37:53Z
license: unknown
score: 8
domains: [audio-engineering, cpp]
tags: [cmake, juce, cpp, audio-plugin]
curated: 2026-06-15
curated_by: config-scout
---

# djrobson/ReverbWave — claude-md

**Why it's worth keeping:** Explicitly lists build targets and artifact paths to prevent guesswork during compilation. Includes high-value 'tribal knowledge' regarding case-sensitive directory naming quirks and target-specific makes.

**Summary:** Provides detailed CMake build commands, target-specific instructions, and output locations essential for JUCE audio development. Maps the project's structural hierarchy and key class responsibilities.

**Source credibility:** Low repo visibility; likely a personal or small-scale project by an individual contributor.

**Recency:** Very current, updated within the last 3 months.

**Source:** [djrobson/ReverbWave/CLAUDE.md](https://github.com/djrobson/ReverbWave/blob/9349166e83e4455ce64c19d9dfd0363277807597/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

ReverbWave is a professional C++ audio reverb effect plugin built with the JUCE framework. It features a sophisticated reverb algorithm based on the Schroeder design with comb and allpass filters, real-time spectrum analysis, and harmonic detuning for enhanced stereo imaging.

## Build System

This project uses CMake as its primary build system:

### Basic Build Commands
```bash
# Configure and build (Release)
mkdir -p build && cd build
cmake .. -DCMAKE_BUILD_TYPE=Release
make

# For Windows
cmake --build . --config Release

# Build specific targets
make ReverbWave                    # Main plugin target
make ReverbWave_VST3              # VST3 plugin only
make ReverbWave_Standalone        # Standalone app only  
make ReverbWave_AU                # Audio Unit (macOS)
```

### Output Locations
- VST3 Plugin: `build/ReverbWave_artefacts/VST3/`
- Standalone App: `build/ReverbWave_artefacts/Standalone/`
- AU Plugin: `build/ReverbWave_artefacts/AU/` (macOS)

## Project Architecture

### Core Components

**Source Directory Structure:**
- `Source/Plugin
```

</details>
