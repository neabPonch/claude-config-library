---
name: VitalikPro13__HOLLOW
source: https://github.com/VitalikPro13/HOLLOW/blob/bbf91aa551c4eefdf19507f770d9c91c7dc0bf46/CLAUDE.md
repo: VitalikPro13/HOLLOW
kind: claude-md
stars: 6
last_pushed: 2026-06-15T18:03:20Z
license: agpl-3.0
score: 9
domains: [mobile-app, systems-programming, security]
tags: [flutter, rust, ffi, e2ee, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# VitalikPro13/HOLLOW — claude-md

**Why it's worth keeping:** The 'Key Architecture Notes' section provides specific implementation warnings to prevent logic errors, while the detailed file tree maps functional responsibility to directory structure.

**Summary:** A highly detailed guide for a complex Flutter/Rust hybrid project covering architecture, FFI workflows, and custom design system constraints.

**Source credibility:** High; demonstrates deep technical complexity in E2EE and cross-language FFI.

**Recency:** 

**Source:** [VitalikPro13/HOLLOW/CLAUDE.md](https://github.com/VitalikPro13/HOLLOW/blob/bbf91aa551c4eefdf19507f770d9c91c7dc0bf46/CLAUDE.md) · 6★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# HOLLOW — Project Instructions for Claude Code

## What Is This
Hollow is a fully distributed, encrypted Discord alternative. No central servers. Members collectively host the server. See `HOLLOW_PLAN.md` for the full architecture, phase history, and current TODO checklist.

## Tech Stack
- **UI:** Flutter (Dart) — all platforms (Windows, macOS, Linux, Android, iOS, Web)
- **Backend:** Rust via `flutter_rust_bridge` v2.11.1 FFI
- **Networking:** WSS relay (signaling + text/CRDT/MLS) + WebRTC data channels (files/shards P2P) + WebRTC media (voice/video P2P). libp2p fully removed.
- **E2EE:** vodozemac (Olm/Double Ratchet) for DMs, OpenMLS 0.8 for servers, SFrame (AES-128-GCM) for voice/video/screen share
- **Local DB:** SQLCipher (encrypted SQLite)
- **Identity:** Ed25519 keypairs via BIP-39 mnemonic (ed25519-dalek, NativeKeypair)
- **Org ID:** com.anonlisten
- **Project name:** hollow

## Project Structure
```
HOLLOW/
├── lib/                  # Dart/Flutter code (UI, app logic, state management)
│   ├── main.dart         # Entry point (ProviderScope + RustLib.init + window_manager init)
│   └── src/
│       ├── core/         # Models, Riverpod providers, service wrappers
│
```

</details>
