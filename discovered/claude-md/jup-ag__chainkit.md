---
name: jup-ag__chainkit
source: https://github.com/jup-ag/chainkit/blob/cdf89cfe3b72595ed4035c5201a3e2cc439ed421/CLAUDE.MD
repo: jup-ag/chainkit
kind: claude-md
stars: 2
last_pushed: 2026-05-09T08:39:22Z
license: unknown
score: 9
domains: [rust, blockchain, systems-programming]
tags: [uniffi, cross-platform, solana]
curated: 2026-06-15
curated_by: config-scout
---

# jup-ag/chainkit — claude-md

**Why it's worth keeping:** The detailed directory tree provides perfect spatial awareness for the agent, while specific build commands and optimization flags enable autonomous compilation and testing.

**Summary:** A high-density architectural blueprint for a complex cross-platform Rust/UniFFI project. It bridges the gap between low-level source code and high-level build/distribution processes.

**Source credibility:** High; maintained by Jup-AG (Jupiter), a major player in the Solana ecosystem.

**Recency:** Very current, with updates from within the last month.

**Source:** [jup-ag/chainkit/CLAUDE.MD](https://github.com/jup-ag/chainkit/blob/cdf89cfe3b72595ed4035c5201a3e2cc439ed421/CLAUDE.MD) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# ChainKit - Project Documentation for Claude

## Project Overview

ChainKit is a cross-platform blockchain utility library providing native interfaces for both iOS/macOS and Android platforms. Built with Rust at its core, it offers high-performance cryptographic and blockchain utilities with native bindings for Swift and Kotlin using Mozilla's UniFFI framework.

**Primary Purpose**: Provide a unified, performant, and secure interface for blockchain operations (primarily Solana) across mobile platforms.

**GitHub Repository**: https://github.com/jup-ag/chainkit

## Architecture

### Core Technology Stack

- **Core Language**: Rust (Edition 2021)
- **FFI Bridge**: Mozilla UniFFI 0.26.1
- **Target Platforms**:
  - iOS/macOS (via Swift)
  - Android (via Kotlin/JNI)
- **Blockchain**: Solana SDK 1.15.2

### Project Structure

```
chainkit/
├── src/                          # Rust core implementation
│   ├── lib.rs                    # Main library entry point
│   ├── interface.udl             # UniFFI interface definition
│   ├── types.rs                  # Core type definitions and traits
│   ├── types_impl.rs             # Type implementations
│   ├── errors.rs                 # Error
```

</details>
