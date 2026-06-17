---
name: minnow54426__minnow54426.github.io
source: https://github.com/minnow54426/minnow54426.github.io/blob/c3850f004676bb19f3be3dc3c6680d7f55aab7d3/CLAUDE.md
repo: minnow54426/minnow54426.github.io
kind: claude-md
stars: 0
last_pushed: 2026-05-23T03:20:50Z
license: other
score: 8
domains: [web-frontend, rust, media-processing]
tags: [portfolio, rust, ffmpeg, github-pages]
curated: 2026-06-15
curated_by: config-scout
---

# minnow54426/minnow54426.github.io — claude-md

**Why it's worth keeping:** Includes highly actionable domain knowledge like FFmpeg settings for size constraints and detailed CSS template architecture descriptions.

**Summary:** Provides comprehensive build commands for a multi-crate Rust workspace and specific media compression workflows.

**Source credibility:** Personal portfolio repository with high manual detail despite low social proof.

**Recency:** Current; references recent model versions and modern toolchains.

**Source:** [minnow54426/minnow54426.github.io/CLAUDE.md](https://github.com/minnow54426/minnow54426.github.io/blob/c3850f004676bb19f3be3dc3c6680d7f55aab7d3/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

Personal portfolio website with GitHub Pages, featuring photography, code projects (Zero Knowledge Proof learning and Groth16 implementation), and interactive cryptography visualizations.

## Key Commands

### Local Development
```bash
# Start local development server (from repository root)
python -m http.server 8001

# View local site
# Main page: http://localhost:8001/
# Photo gallery: http://localhost:8001/photo-gallery.html
# Paint gallery: http://localhost:8001/paint.html
# Code projects: http://localhost:8001/code.html
# Polynomial plotter: http://localhost:8001/cryptography/polynomial-plotter.html
# Music: http://localhost:8001/music.html
```

### Rust Projects

#### Groth16 Demo (Code Project)
```bash
# Navigate to project
cd code/groth16-demo

# Build workspace
cargo build

# Run tests
cargo test

# Run tests with output
cargo test -- --nocapture

# Run specific test
cargo test test_name

# Run clippy for linting
cargo clippy

# Format code
cargo fmt

# Generate documentation
cargo doc --open

# Run benchmarks
cargo bench

# Build mdbook documentation
mdbook
```

</details>
