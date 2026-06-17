---
name: Dilaz__norppalive_service
source: https://github.com/Dilaz/norppalive_service/blob/ead0803e494b8cdcbf3b2fd27d7cdee2c9c9a1e0/CLAUDE.md
repo: Dilaz/norppalive_service
kind: claude-md
stars: 0
last_pushed: 2026-06-02T12:17:20Z
license: mit
score: 9
domains: [backend, rust, computer-vision]
tags: [rust, actor-model, video-processing]
curated: 2026-06-16
curated_by: config-scout
---

# Dilaz/norppalive_service — claude-md

**Why it's worth keeping:** The inclusion of an architecture diagram, categorized test commands, and a step-by-step 'Adding a New Service' guide ensures pattern consistency when the AI extends the code.

**Summary:** Provides clear architectural mental models through ASCII diagrams and explicit workflows for system expansion.

**Source credibility:** Low social proof (0 stars), but demonstrates high technical competence in documentation structure.

**Recency:** 

**Source:** [Dilaz/norppalive_service/CLAUDE.md](https://github.com/Dilaz/norppalive_service/blob/ead0803e494b8cdcbf3b2fd27d7cdee2c9c9a1e0/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Norppalive Service detects Saimaa ringed seals from the Finnish WWF Norppalive livestream using an actor-based architecture (Actix). It processes video frames through an AI detection API and posts findings to social media platforms (Twitter, Mastodon, Bluesky) and Kafka.

## Build & Run Commands

```bash
cargo build                           # Debug build
cargo build --release                 # Release build (optimized for size with LTO)
cargo run                             # Run with default config.toml
cargo run -- --config <path>          # Run with custom config file
```

## Testing

```bash
cargo test                            # Run all tests
cargo test -- --nocapture             # Show println! output
cargo test <name>                     # Run specific test by name

# Test categories
cargo test actors                     # Actor tests
cargo test integration_tests          # Integration tests
cargo test supervisor                 # SupervisorActor tests
cargo test detection                  # DetectionActor tests
cargo test stream
```

</details>
