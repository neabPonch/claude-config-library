---
name: decentraland__godot-explorer
source: https://github.com/decentraland/godot-explorer/blob/599f9503afa679836e89d6d8a447f7add4188dcf/CLAUDE.md
repo: decentraland/godot-explorer
kind: claude-md
stars: 17
last_pushed: 2026-06-15T17:09:27Z
license: apache-2.0
score: 9
domains: [game-engine, rust, cross-platform]
tags: [godot, rust, xtask, systems]
curated: 2026-06-15
curated_by: config-scout
---

# decentraland/godot-explorer — claude-md

**Why it's worth keeping:** It utilizes the 'xtask' pattern to abstract all tooling through cargo commands and provides specific environmental optimization tips, such as stripping iOS templates to save disk space.

**Summary:** A highly detailed technical guide for a complex Rust/Godot project requiring multi-platform builds for Android, iOS, and desktop.

**Source credibility:** High; part of a professional decentralized metaverse project with active maintenance.

**Recency:** Very current, referencing Godot 4.6 and modern development workflows.

**Source:** [decentraland/godot-explorer/CLAUDE.md](https://github.com/decentraland/godot-explorer/blob/599f9503afa679836e89d6d8a447f7add4188dcf/CLAUDE.md) · 17★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Decentraland Godot Explorer is a cross-platform metaverse client that combines:
- **Godot Engine 4.6.2** (custom fork) for 3D rendering and UI
- **Rust** for core systems and performance-critical components
- **GDScript** for game logic
- **JavaScript/V8** runtime for executing Decentraland SDK scenes

## Essential Commands

All commands use the xtask pattern via `cargo run --`:

### System Health & Dependencies
```bash
# Check system health and dependencies
cargo run -- doctor

# Install dependencies (specify platforms: linux, windows, macos, android, ios)
cargo run -- install                      # Installs protoc and Godot only (fresh download)
cargo run -- install --targets linux      # Also installs Linux export templates
cargo run -- install --targets android    # Also installs Android tools and templates
cargo run -- install --targets ios        # iOS templates (keeps debug symbols)
cargo run -- install --targets ios --strip-ios  # iOS templates (strips debug symbols to save disk)
cargo run -- install --cache              # Use cached down
```

</details>
