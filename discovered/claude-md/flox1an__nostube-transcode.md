---
name: flox1an__nostube-transcode
source: https://github.com/flox1an/nostube-transcode/blob/d26923563a7b036564b8bad41be2bae962ace6e1/CLAUDE.md
repo: flox1an/nostube-transcode
kind: claude-md
stars: 1
last_pushed: 2026-05-05T08:25:34Z
license: unknown
score: 9
domains: [rust, media-processing, backend]
tags: [rust, ffmpeg, architecture-documentation, workflow]
curated: 2026-06-16
curated_by: config-scout
---

# flox1an/nostube-transcode — claude-md

**Why it's worth keeping:** The inclusion of a step-by-step Data Flow section and a logical Startup Sequence provides essential context for an AI to debug complex state transitions. The module breakdowns provide clear semantic meaning to the file structure beyond just names.

**Summary:** A highly detailed technical blueprint that maps out not just how to run the code, but how data flows through specific modules and how the system initializes.

**Source credibility:** Small project (1 star) but contains high-density, professional-grade technical documentation.

**Recency:** Very recent (last pushed 1 month ago), making it perfectly aligned with modern Claude Code workflows.

**Source:** [flox1an/nostube-transcode/CLAUDE.md](https://github.com/flox1an/nostube-transcode/blob/d26923563a7b036564b8bad41be2bae962ace6e1/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

A Nostr Data Vending Machine (DVM) that transforms videos into HLS format and uploads them to Blossom servers. The DVM listens for video transformation requests on Nostr relays, processes videos using FFmpeg, and publishes results back to the network.

## Build & Run Commands

```bash
# Build and run
cargo run

# Build release
cargo build --release

# Run tests
cargo test

# Run specific test
cargo test test_ffmpeg_command

# Check/lint
cargo check
cargo clippy
cargo fmt --check

# With debug logging
RUST_LOG=nostube_transcode=debug cargo run
```

### Frontend (React/Vite in `frontend/`)

```bash
cd frontend
npm install
npm run dev      # Development server
npm run build    # Production build (output embedded in Rust binary)
npm run lint
```

## Architecture

### Core Components

- **main.rs** - Entry point, initializes DVM in remote config mode
- **config.rs** - Configuration from remote Nostr config (NIP-78)
- **lib.rs** - Re-exports all modules for testing

### Module Structure

- **dvm/** - Nostr DVM protocol handling
  - `handler.rs` - Job p
```

</details>
