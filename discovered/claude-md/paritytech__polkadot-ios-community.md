---
name: paritytech__polkadot-ios-community
source: https://github.com/paritytech/polkadot-ios-community/blob/51268d146910cd989e37a1d2286648c4af278854/CLAUDE.md
repo: paritytech/polkadot-ios-community
kind: claude-md
stars: 4
last_pushed: 2026-06-13T00:10:18Z
license: gpl-3.0
score: 9
domains: [ios, mobile-app, swift]
tags: [viper, xcodebuild, architectural-constraints, swift]
curated: 2026-06-15
curated_by: config-scout
---

# paritytech/polkadot-ios-community — claude-md

**Why it's worth keeping:** It provides specific 'negative constraints' (e.g., max nesting/parameters) to enforce code quality and explains complex data flow logic like the CoreData mapper pattern to prevent race conditions.

**Summary:** A high-density guide for a VIPER-structured iOS project that includes build commands, scaffolding scripts, and strict architectural patterns.

**Source credibility:** High; the repo is active, well-structured, and focuses on a specialized blockchain domain.

**Recency:** Very recent, targeting iOS 17 and modern Swift concurrency/patterns.

**Source:** [paritytech/polkadot-ios-community/CLAUDE.md](https://github.com/paritytech/polkadot-ios-community/blob/51268d146910cd989e37a1d2286648c4af278854/CLAUDE.md) · 4★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Polkadot iOS — a production-grade iOS wallet and social app for the Polkadot blockchain ecosystem. Features include wallet management, cross-chain transfers (XCM), real-time chat with WebRTC calls, fiat on-ramp, identity/username claiming, and QR-based interactions.

### Key Technologies
- **UIKit** — Primary UI framework, programmatic layout (no Storyboards)
- **SnapKit** — Auto Layout constraints
- **VIPER** — Architecture pattern for all feature modules
- **Swift Package Manager** — 28 local packages under `Packages/`
- **substrate-sdk-ios** — Substrate/Polkadot blockchain interaction
- **CoreData** — Local persistence (SubstrateDataModel + UserDataModel)
- **WebRTC** — Peer-to-peer voice/video calls and DIM2 game
- **Firebase** — Remote Config

> Build-time configuration and publishing (signing, TestFlight, Firebase App
> Distribution) are documented in [docs/PUBLISHING.md](./docs/PUBLISHING.md).
> This repo ships no hosted CI/CD pipeline or Fastlane implementation; secrets
> and endpoints are externalised into environment variables (see that
```

</details>
