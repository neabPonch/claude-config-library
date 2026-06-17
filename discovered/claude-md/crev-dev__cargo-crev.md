---
name: crev-dev__cargo-crev
source: https://github.com/crev-dev/cargo-crev/blob/bc46f07042dbbc18336a9cd203ebca614c89b36f/CLAUDE.md
repo: crev-dev/cargo-crev
kind: claude-md
stars: 2310
last_pushed: 2026-05-20T22:11:00Z
license: apache-2.0
score: 8
domains: [cli-tools, rust, security]
tags: [rust, cargo, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# crev-dev/cargo-crev — claude-md

**Why it's worth keeping:** The explicit 'layering' dependency constraints are critical for preventing an AI from introducing invalid cross-crate imports.

**Summary:** Provides strict architectural layering rules, specific build/test commands, and a detailed filesystem map.

**Source credibility:** High; a well-regarded Rust project with significant community traction (2300+ stars).

**Recency:** Current; aligns with modern Rust edition and toolchain standards.

**Source:** [crev-dev/cargo-crev/CLAUDE.md](https://github.com/crev-dev/cargo-crev/blob/bc46f07042dbbc18336a9cd203ebca614c89b36f/CLAUDE.md) · 2310★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# cargo-crev

Cryptographically verifiable code review system for the Rust/Cargo ecosystem.
Implements the Crev protocol: Ed25519-signed code reviews + a distributed Web of Trust.

## Workspace Structure (strict layering, low → high)

1. **crev-common** — Shared utilities: blake2b256 hashing, filesystem helpers, YAML I/O
2. **crev-data** — Core data types: proofs, identities, trust levels, cryptographic signing (ed25519-dalek)
3. **crev-wot** — Web of Trust engine: trust set computation, review aggregation
4. **crev-lib** — Library API (like libgit2 for Crev): local proof store, identity management, git-backed repos
5. **cargo-crev** — CLI binary: Cargo subcommand, dependency analysis, crates.io integration

Each layer may only depend on layers below it. The `crevette` crate is excluded from the workspace.

## Building & Testing

```sh
cargo build                    # build all crates
cargo test                     # run all tests
cargo clippy --workspace       # lint
cargo fmt --all                # format
```

Nix environment: `nix develop` (sets up toolchain, rust-analyzer, git hooks).

## Key Dependencies

- `ed25519-dalek` — cryptographic signing
- `git2` — proof repository st
```

</details>
