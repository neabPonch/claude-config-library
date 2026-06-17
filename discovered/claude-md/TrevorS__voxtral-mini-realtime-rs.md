---
name: TrevorS__voxtral-mini-realtime-rs
source: https://github.com/TrevorS/voxtral-mini-realtime-rs/blob/2930e95d60f8584b5326d90d3c5ec9a152d0d322/CLAUDE.md
repo: TrevorS/voxtral-mini-realtime-rs
kind: claude-md
stars: 792
last_pushed: 2026-04-02T20:12:56Z
license: apache-2.0
score: 10
domains: [rust, ml-inference, wasm, audio-processing, gpu-programming]
tags: [rust, webgpu, wasm, gguf, audio]
curated: 2026-06-15
curated_by: config-scout
---

# TrevorS/voxtral-mini-realtime-rs — claude-md

**Why it's worth keeping:** It provides 'reasoning context'—explaining why specific constraints (like peak normalization and WASM memory limits) exist—which prevents an AI from introducing regressions while refactoring.

**Summary:** A highly detailed technical specification for a Rust-based audio inference engine that covers build commands, model weight acquisition, and deep architectural reasoning.

**Source credibility:** High: 792 stars and very recent activity in a specialized Rust/ML domain.

**Recency:** Very current; updated within the last two months.

**Source:** [TrevorS/voxtral-mini-realtime-rs/CLAUDE.md](https://github.com/TrevorS/voxtral-mini-realtime-rs/blob/2930e95d60f8584b5326d90d3c5ec9a152d0d322/CLAUDE.md) · 792★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

direct-commits-allowed: true

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Voxtral Mini 4B Realtime — streaming ASR and TTS in Rust using Burn. Runs natively (Vulkan/Metal) and in the browser (WASM + WebGPU). The Q4 GGUF ASR path enables a 4B-parameter model to run entirely client-side in a browser tab. The TTS pipeline uses Voxtral 4B TTS with 20 preset voices across 9 languages.

## Build & Development Commands

```bash
# Native build
cargo build --features "wgpu,cli,hub"
cargo build --release --features "wgpu,cli,hub"

# WASM build (produces pkg/ directory)
wasm-pack build --target web --no-default-features --features wasm

# Lint both targets
cargo clippy --features "wgpu,cli,hub" -- -D warnings
cargo clippy --no-default-features --features wasm --target wasm32-unknown-unknown -- -D warnings

# Format
cargo fmt
cargo fmt -- --check

# Tests (230 tests: 227 unit + 3 integration)
cargo test --features "wgpu,cli,hub"
cargo test test_q4_roundtrip_small           # single test
cargo test gguf::tests                        # module tests

# Benchmarks (Criterion)
cargo bench --features "wgpu,
```

</details>
