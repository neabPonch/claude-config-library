---
name: gre__gre
source: https://github.com/gre/gre/blob/2328ed2c3277a5562e5326e94a4c10138383d32b/CLAUDE.md
repo: gre/gre
kind: claude-md
stars: 70
last_pushed: 2026-03-21T19:46:23Z
license: mit
score: 9
domains: [web-frontend, rust, creative-coding]
tags: [monorepo, nextjs, generative-art, svg]
curated: 2026-06-15
curated_by: config-scout
---

# gre/gre — claude-md

**Why it's worth keeping:** It includes critical 'gotchas' regarding specific crate versions (rand 0.5.6 syntax) and provides an exact code template for generating new examples, which prevents common LLM hallucinations.

**Summary:** A comprehensive guide for a monorepo containing a Next.js site and Rust-based generative art projects.

**Source credibility:** High; the repository is a well-structured creative coding portfolio by @greweb.

**Recency:** Current; provides up-to-date instructions for both modern Next.js and specific Rust crate requirements.

**Source:** [gre/gre/CLAUDE.md](https://github.com/gre/gre/blob/2328ed2c3277a5562e5326e94a4c10138383d32b/CLAUDE.md) · 70★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Is

Monorepo for **greweb.me** — @greweb's generative plotter art portfolio. Combines a Next.js website with 1500+ Rust generative art examples, experimental doodle projects, shader experiments, and blockchain art.

## Common Commands

### Website (Next.js)

```bash
npm run dev          # Dev server (uses --openssl-legacy-provider for Node compat)
npm run build        # Production build
npm run start        # Start production server
```

### Plots (Rust generative art → SVG for pen plotters)

```bash
cd plots
cargo run --example 001                 # Run a specific plot, outputs image.svg
cargo run --example 001 -- --seed 42    # With specific seed (examples using clap)
cargo watch "run --example 001"         # Hot reload (watch for changes)
```

### Doodles (Rust/WASM generative art projects)

```bash
# From repo root, for a Rust-based doodle:
npm run build-rust-doodle               # Build Rust → WASM (uses scripts/build-rust-doodle.sh)
npm run build-doodle                    # Webpack bundle for web
npm run start-doodle                    # Parcel dev
```

</details>
