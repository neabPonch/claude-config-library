---
name: gclinian__SafeDrop
source: https://github.com/gclinian/SafeDrop/blob/999fa06a0165d16ccde314d4a74edf44b50fb6a6/CLAUDE.md
repo: gclinian/SafeDrop
kind: claude-md
stars: 6
last_pushed: 2026-06-03T02:52:45Z
license: mit
score: 9
domains: [cross-platform, systems-programming, security, network-protocols]
tags: [multi-language, protocol-driven, concurrency-warnings]
curated: 2026-06-15
curated_by: config-scout
---

# gclinian/SafeDrop — claude-md

**Why it's worth keeping:** The 'Single Most Important Rule' regarding protocol synchronization is an elite pattern for cross-platform projects. It also proactively warns against breaking specific threading behaviors in Swift, which prevents AI-driven refactoring errors.

**Summary:** Defines a strict 'single source of truth' via a wire protocol for multi-language interoperability and provides critical platform-specific concurrency caveats.

**Source credibility:** High; the file demonstrates deep systems engineering knowledge regarding I/O and concurrency.

**Recency:** Current; integrates modern concepts like MCP (Model Context Protocol) and mobile frameworks.

**Source:** [gclinian/SafeDrop/CLAUDE.md](https://github.com/gclinian/SafeDrop/blob/999fa06a0165d16ccde314d4a74edf44b50fb6a6/CLAUDE.md) · 6★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What SafeDrop is

A zero-config LAN file + clipboard sharing tool **plus** a Model Context
Protocol fabric. Three native implementations (Python desktop, Kotlin
Android, Swift iOS) speak byte-for-byte the same X25519 + Fernet +
JSON-over-TCP protocol. Authoritative user-facing docs:
[`README.md`](README.md), [`SPEC.md`](SPEC.md),
[`MCP_AGENT_GUIDE.md`](MCP_AGENT_GUIDE.md).

## The single most important rule: the wire protocol is the contract

`SPEC.md` is the source of truth for what goes on the wire. Any change
to it must land in **all three** implementations in the same change
set, and must come with a regression in `tests/test_*_interop.py`. The
interop tests are how we know Python/Kotlin/Swift agree byte-for-byte
on Fernet token format, X25519 + HKDF derivation, and frame layout —
breaking them is how a release goes silently wrong on one platform.

If you're adding a wire-level feature: update `SPEC.md` first, then
mirror in `safedrop/`, `android/app/src/main/java/com/safedrop/android/`,
and `ios/SafeDrop/` simultaneously.

## Architecture orientation

### `sa
```

</details>
