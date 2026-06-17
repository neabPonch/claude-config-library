---
name: deerportal__deerportal
source: https://github.com/deerportal/deerportal/blob/b38430fdfbe036993a94a6b37c68a34cfe6e1d22/CLAUDE.md
repo: deerportal/deerportal
kind: claude-md
stars: 34
last_pushed: 2025-07-30T20:03:10Z
license: other
score: 9
domains: [game-development, graphics, cpp]
tags: [cmake, sfml, architecture, versioning, c++]
curated: 2026-06-16
curated_by: config-scout
---

# deerportal/deerportal — claude-md

**Why it's worth keeping:** The 'Important Files' section creates an excellent roadmap for the AI to navigate deep context, while the explicit versioning/release protocols prevent common agent errors during deployment.

**Summary:** Provides a comprehensive technical blueprint including specific build flags, architectural mapping, and a curated registry of high-context documentation files.

**Source credibility:** A well-structured, specialized game project with professional-grade technical documentation.

**Recency:** Current; uses modern SFML 3.0 and up-to-date C++ standards.

**Source:** [deerportal/deerportal/CLAUDE.md](https://github.com/deerportal/deerportal/blob/b38430fdfbe036993a94a6b37c68a34cfe6e1d22/CLAUDE.md) · 34★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

DeerPortal is a hybrid board/card game built with SFML 3.0 and C++17. It's a cross-platform game supporting 0-4 players with AI opponents, featuring elemental mechanics and card-based gameplay.

**Current Version: 0.10.0-pre.1 "Lighting Effects Development"**  
**Technology Stack: SFML 3.0.1, CMake, C++17**  
**Code Quality: A+ Grade (97/100) - Professional implementation with latest state management fixes**

## Build Commands

### Primary Build System (CMake)
```bash
# Configure for Release (recommended)
cmake -DCMAKE_BUILD_TYPE=Release .

# Configure for Debug (development)
cmake -DCMAKE_BUILD_TYPE=Debug .

# Enable FPS counter in Release build
cmake -DCMAKE_BUILD_TYPE=Release -DSHOW_FPS_COUNTER=ON .

# Build executable
make

# Create platform packages
make package         # Cross-platform packages
make dmg            # macOS DMG installer  
make install        # Install to system
```

### Version Management
- **Single source of truth**: `version.txt` contains current version
- **Manual updates required**: `snapcraft.yaml`, `net.devcarpet.deerp
```

</details>
