---
name: bitwarden__sdk-sm__claude
source: https://github.com/bitwarden/sdk-sm/blob/2f2c866e87420dcdebfbf6f887d32b8c726a67f4/.claude/CLAUDE.md
repo: bitwarden/sdk-sm
kind: claude-md
stars: 437
last_pushed: 2026-06-13T02:47:20Z
license: other
score: 8
domains: [rust, security, cli-tools]
tags: [monorepo, cross-language, schema-driven]
curated: 2026-06-15
curated_by: config-scout
---

# bitwarden/sdk-sm — claude-md

**Why it's worth keeping:** Includes explicit linting constraints (denying unwrap/unused_async), precise build commands for various targets, and explains the critical schema-driven workflow used to update language bindings.

**Summary:** Provides a comprehensive architectural blueprint and specific operational workflows for a multi-language Rust SDK.

**Source credibility:** High; Bitwarden is an established security company with a highly maintained repository.

**Recency:** Very current, referencing Rust 1.85 and modern development toolchains.

**Source:** [bitwarden/sdk-sm/.claude/CLAUDE.md](https://github.com/bitwarden/sdk-sm/blob/2f2c866e87420dcdebfbf6f887d32b8c726a67f4/.claude/CLAUDE.md) · 437★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Bitwarden Secrets Manager SDK

## Crates

The project is structured as a monorepo using cargo workspaces. Some of the more noteworthy crates
are:

- [`bitwarden`](./crates/bitwarden/): Rust-friendly API for interacting with the secrets manager.
- [`bitwarden-c`](./crates/bitwarden-c/): C bindings for FFI interop.
- [`bitwarden-json`](./crates/bitwarden-json/): JSON wrapper around the `bitwarden` crate. Powers
  the other language bindings.
- [`bitwarden-napi`](./crates/bitwarden-napi/): Node-API bindings for Node.js/TypeScript.
- [`bitwarden-wasm`](./crates/bitwarden-wasm/): WebAssembly bindings.
- [`bws`](./crates/bws/): CLI for interacting with the [Bitwarden Secrets Manager][secrets-manager].
  Review the [CLI documentation][bws-help].
- [`sdk-schemas`](./crates/sdk-schemas/): Generator for the _json schemas_.
- [`fake-server`](./crates/fake-server/): Development/testing server that emulates Bitwarden API
  endpoints for local testing without a real server instance.

### Language Bindings

The SDK provides bindings in the `/languages/` directory: C++, C#, Go, Java, JavaScript/TypeScript,
PHP, Python, and Ruby. All bindings share a consistent API for projects and secrets manage
```

</details>
