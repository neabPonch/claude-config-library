---
name: erssi-org__erssi__claude
source: https://github.com/erssi-org/erssi/blob/c591e6c09bece85e532aa9e23eddf8a07eaea7ee/docs/postdev/CLAUDE.md
repo: erssi-org/erssi
kind: claude-md
stars: 1
last_pushed: 2026-05-18T04:43:50Z
license: other
score: 8
domains: [cli-tools, systems-programming, c]
tags: [build-system, architecture-mapping, low-level]
curated: 2026-06-15
curated_by: config-scout
---

# erssi-org/erssi — claude-md

**Why it's worth keeping:** It includes 'Common Development Tasks' which proactively instructs the AI on implementation patterns and logic flows across multiple files.

**Summary:** Provides detailed architectural mapping and specific build/development workflows for a specialized C project.

**Source credibility:** Single-star repo, likely an individual developer's custom work.

**Recency:** Highly current; last pushed 1 month ago.

**Source:** [erssi-org/erssi/docs/postdev/CLAUDE.md](https://github.com/erssi-org/erssi/blob/c591e6c09bece85e532aa9e23eddf8a07eaea7ee/docs/postdev/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is **Evolved Irssi (erssi)** - a modernized IRC client based on the classic irssi with enhanced features while maintaining full compatibility. The project version is `1.5-erssi-v0.0.5` and uses the Meson build system.

## Build Commands

### Development Build
```bash
meson setup Build --prefix=/opt/erssi -Dwith-perl=yes -Dwith-otr=yes -Ddisable-utf8proc=no
ninja -C Build
```

### Installation (requires sudo for global install)
```bash
sudo ninja -C Build install
```

### Testing
```bash
# Run tests from build directory
ninja -C Build test
```

### Clean Build
```bash
rm -rf Build
```

## Key Architecture Components

### Core Systems
- **Sidepanel System** (`src/fe-ansi/sidepanels*`): Modular architecture with separate left (window list) and right (nicklist) panels
  - `sidepanels-core.c`: Main coordination and settings management
  - `sidepanels-render.c`: Rendering logic with optimized redraw functions
  - `sidepanels-activity.c`: Activity tracking and batch processing
  - `sidepanels-signals.c`: IRC event signal handling
  - `sidepanels-la
```

</details>
