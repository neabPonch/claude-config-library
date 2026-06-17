---
name: trustwallet__wallet-core
source: https://github.com/trustwallet/wallet-core/blob/a4e9c6b3f0673bb60664e8879c2c6c16742726e5/CLAUDE.md
repo: trustwallet/wallet-core
kind: claude-md
stars: 3526
last_pushed: 2026-06-15T11:40:48Z
license: apache-2.0
score: 10
domains: [systems-programming, blockchain, cross-platform]
tags: [architecture-map, build-system, multi-language, codegen]
curated: 2026-06-15
curated_by: config-scout
---

# trustwallet/wallet-core — claude-md

**Why it's worth keeping:** It explicitly defines 'safe' vs. 'auto-generated' code zones and explains the specific logic required to register new modules using internal markers like #coin-list#.

**Summary:** Provides exhaustive command sets for multi-language builds and a deep architectural map of how data flows from C++ through language bindings.

**Source credibility:** High; Trust Wallet Core is a major, highly-starred industry standard for blockchain security.

**Recency:** Highly current; reflects very recent repository activity.

**Source:** [trustwallet/wallet-core/CLAUDE.md](https://github.com/trustwallet/wallet-core/blob/a4e9c6b3f0673bb60664e8879c2c6c16742726e5/CLAUDE.md) · 3526★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Is

Trust Wallet Core is a cross-platform C++ library implementing cryptographic wallet functionality for 130+ blockchains. The C++ core exposes a strict C ABI (`TW*` functions in `include/TrustWalletCore/`) from which language bindings for Swift, Kotlin, TypeScript/WASM, and Rust are auto-generated.

---

## Commands

### C++ (primary)

```bash
# First-time setup
./bootstrap.sh

# Full build + test (standard dev loop)
tools/build-and-test

# Or step by step:
tools/generate-files native          # must run after any .proto or registry.json change
cmake -H. -Bbuild -DCMAKE_BUILD_TYPE=Debug -DCMAKE_C_COMPILER=clang -DCMAKE_CXX_COMPILER=clang++
make -Cbuild -j12 tests TrezorCryptoTests

# Run all C++ tests
./build/tests/tests

# Run a single test or filter
./build/tests/tests --gtest_filter="*Bitcoin*"
./build/tests/tests --gtest_filter="*Ethereum*SignTest*"

# Run TrezorCrypto tests (low-level crypto primitives)
export CK_TIMEOUT_MULTIPLIER=4
./build/trezor-crypto/crypto/tests/TrezorCryptoTests

# Lint changed files (clang-tidy, diffs against master)
tools
```

</details>
