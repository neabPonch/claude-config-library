---
name: napi-rs__napi-rs
source: https://github.com/napi-rs/napi-rs/blob/529a78d15c0c7d6ca6d4a732c5e335f9de701879/CLAUDE.md
repo: napi-rs/napi-rs
kind: claude-md
stars: 7783
last_pushed: 2026-06-14T09:59:42Z
license: other
score: 7
domains: [rust, nodejs, cli-tools, systems-programming]
tags: [monorepo, ff-bindings, build-process]
curated: 2026-06-15
curated_by: config-scout
---

# napi-rs/napi-rs — claude-md

**Why it's worth keeping:** Provides specific, high-utility commands for type generation and snapshot updates that are crucial for maintaining toolchain consistency.

**Summary:** Outlines the multi-language build and test workflow for a Rust-to-Node.js bridge.

**Source credibility:** High; napi-rs is a widely used industry standard with significant community backing.

**Recency:** Very current; the repository shows active maintenance.

**Source:** [napi-rs/napi-rs/CLAUDE.md](https://github.com/napi-rs/napi-rs/blob/529a78d15c0c7d6ca6d4a732c5e335f9de701879/CLAUDE.md) · 7783★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# NAPI-RS Project Guide

## Project Structure

**Core Architecture:**

- `/crates/` - Rust implementation
  - `napi/` - Main runtime library (Node-API bindings)
  - `napi-sys/` - Low-level FFI bindings
  - `macro/` - Procedural macros (`#[napi]` attributes)
  - `backend/` - Code generation and TypeScript definitions
  - `build/` - Build utilities
- `/cli/` - Command-line tool (@napi-rs/cli)
- `/examples/napi/` - Comprehensive test suite and examples
- Monorepo using Cargo workspaces (Rust) + Yarn workspaces (JS)

**Key Files:**

- Root `Cargo.toml` - Workspace configuration
- `/crates/backend/src/typegen.rs` - TypeScript generation logic
- `/cli/src/utils/typegen.ts` - CLI TypeScript processing

## Testing, Building, and Running Tests

### Building

```bash
# Build all tests
yarn build:tests

# Build specific example (most common for testing changes)
yarn workspace @examples/napi build
```

### Testing

```bash
# Run all tests in the example project
yarn workspace @examples/napi test

# Update test snapshots after changes
yarn workspace @examples/napi test -u

# Run specific test file
yarn workspace @examples/napi test __tests__/values.spec.ts

# Run Rust unit tests
cargo test

# R
```

</details>
