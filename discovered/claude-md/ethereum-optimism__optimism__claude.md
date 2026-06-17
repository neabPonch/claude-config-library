---
name: ethereum-optimism__optimism__claude
source: https://github.com/ethereum-optimism/optimism/blob/3a7401b913974c0cf7edc938cd02efa9009d179e/rust/kona/CLAUDE.md
repo: ethereum-optimism/optimism
kind: claude-md
stars: 6447
last_pushed: 2026-06-15T03:57:21Z
license: mit
score: 9
domains: [systems-programming, blockchain, rust]
tags: [monorepo, rust-toolchain, architecture-mapping]
curated: 2026-06-15
curated_by: config-scout
---

# ethereum-optimism/optimism — claude-md

**Why it's worth keeping:** The architectural breakdown of the monorepo is a masterclass in providing context for LLMs navigating complex directory structures; the strict 'no warnings' and MSRV specifications ensure AI output adheres to high-integrity standards.

**Summary:** A high-density guide for a Rust monorepo that maps specific task runner commands to architectural components.

**Source credibility:** High; originated from a top-tier Ethereum infrastructure repository with significant community backing.

**Recency:** Current; uses modern Rust toolchain practices, nextest, and specific task runner patterns used in active development.

**Source:** [ethereum-optimism/optimism/rust/kona/CLAUDE.md](https://github.com/ethereum-optimism/optimism/blob/3a7401b913974c0cf7edc938cd02efa9009d179e/rust/kona/CLAUDE.md) · 6447★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Build Commands
- Build workspace: `just b` or `just build-native`
- Lint: `just l` or `just lint-native`
- Format: `just f` or `just fmt-native-fix` (if `rust-fmt` CI fails, use `/fix-rust-fmt`)
- Run all tests: `just t` or `just tests`
- Run specific test: `cargo nextest run --package [package-name] --test [test-name]`
- Run single test: `cargo nextest run --package [package-name] --test [test-name] -- [test_function_name]`
- Documentation: `just test-docs`

## Code Style
- MSRV: 1.92
- Format with nightly rustfmt: `cargo +nightly fmt`
- Imports: organized by crate, reordered automatically
- Error handling: use proper error types, prefer `Result<T, E>` over panics
- Naming: follow Rust conventions (snake_case for variables/functions, CamelCase for types)
- Prefer type-safe APIs and strong typing
- Documentation: rustdoc for public APIs, clear comments for complex logic
- Tests: write unit and integration tests for all functionality
- Performance: be mindful of allocations and copying, prefer references where appropriate
- No warnings policy: all clippy warnings a
```

</details>
