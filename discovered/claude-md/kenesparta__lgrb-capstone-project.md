---
name: kenesparta__lgrb-capstone-project
source: https://github.com/kenesparta/lgrb-capstone-project/blob/08c214cc81e5a26eea5c0c2a64562bf85761713c/CLAUDE.md
repo: kenesparta/lgrb-capstone-project
kind: claude-md
stars: 1
last_pushed: 2026-01-28T06:33:03Z
license: unknown
score: 9
domains: [embedded, iot, rust, backend]
tags: [iot, rust-embedded, cross-compilation, hardware-simulation]
curated: 2026-06-15
curated_by: config-scout
---

# kenesparta/lgrb-capstone-project — claude-md

**Why it's worth keeping:** Provides critical simulation instructions (curl mocks) to test the backend without hardware and includes specific cross-compilation/flashing commands for embedded targets. The architecture diagram and GATT service mapping provide essential context for an LLM to understand the system loop.

**Summary:** A comprehensive guide for a multi-crate Rust IoT system involving embedded firmware, BLE communication, and a web server.

**Source credibility:** Low star count, but highly structured and useful capstone project documentation.

**Recency:** Recent (5 months ago) and uses modern Rust tooling/workflows.

**Source:** [kenesparta/lgrb-capstone-project/CLAUDE.md](https://github.com/kenesparta/lgrb-capstone-project/blob/08c214cc81e5a26eea5c0c2a64562bf85761713c/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

LGRB (Let's Get Rusty) Capstone Project - A multi-crate Rust IoT system connecting a BBC micro:bit v2 to a real-time web
dashboard via Bluetooth Low Energy.

**Architecture:**

```
micro:bit v2 (lgrcp-embed) → BLE → ble-listener → HTTP POST → ws-server → WebSocket → Browser
```

## Build Commands

### WebSocket Server (ws-server)

```bash
cargo run -p ws-server              # Debug, listens on 0.0.0.0:3000
cargo run -p ws-server --release    # Release
```

### BLE Listener (ble-listener)

```bash
cargo run -p ble-listener           # Requires Bluetooth adapter + device advertising "LGR-BLE"
cargo run -p ble-listener --release
```

### Embedded Firmware (lgrcp-embed)

```bash
# Install toolchain first
cd lgrcp-embed && make prepare

# Build
cargo build --release --target thumbv7em-none-eabihf -p lgrcp-embed

# Flash to micro:bit v2
cargo flash --chip nRF52833_xxAA --release --target thumbv7em-none-eabihf -p lgrcp-embed
```

### Cross-Compilation (Raspberry Pi aarch64)

```bash
rustup target add aarch64-unknown-linux-gnu
make build-ws-server      #
```

</details>
