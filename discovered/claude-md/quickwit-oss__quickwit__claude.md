---
name: quickwit-oss__quickwit__claude
source: https://github.com/quickwit-oss/quickwit/blob/74b39ac1cdc98d8efcc65d863ce43d98acaa967d/quickwit/CLAUDE.md
repo: quickwit-oss/quickwit
kind: claude-md
stars: 11320
last_pushed: 2026-06-15T12:28:42Z
license: apache-2.0
score: 9
domains: [backend, rust, distributed-systems]
tags: [rust, architecture-mapping, negative-constraints]
curated: 2026-06-15
curated_by: config-scout
---

# quickwit-oss/quickwit — claude-md

**Why it's worth keeping:** It utilizes negative constraints (banned methods) and highly specific stylistic rules (log formatting) to ensure AI output matches production standards. The crate-to-layer mapping provides critical structural context.

**Summary:** A comprehensive guide for a large Rust workspace that links architectural layers to specific crates and build procedures.

**Source credibility:** High; the source is a highly-starred, actively maintained cloud-native search engine.

**Recency:** Current; includes specific toolchain versions and modern Rust development practices.

**Source:** [quickwit-oss/quickwit/quickwit/CLAUDE.md](https://github.com/quickwit-oss/quickwit/blob/74b39ac1cdc98d8efcc65d863ce43d98acaa967d/quickwit/CLAUDE.md) · 11320★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
## Build & Test Commands

### Formatting & Linting
- **`make fmt`** — Format and validate code (requires nightly toolchain: `rustup toolchain install nightly`):
  1. Runs `cargo +nightly fmt`
  2. Checks license headers on `.rs`, `.ts`, `.proto` files
  3. Enforces log format policy: no trailing punctuation, no uppercase first character in log and error messages
- **`make fix`** — Runs clippy with `--fix`, then `make fmt`, then `make unused-deps`
- **`make unused-deps`** — Detects unused dependencies via `cargo-machete`

Log messages (`info!`, `warn!`, `error!`, `debug!`) must:
- Start with a **lowercase** letter
- Have **no trailing punctuation**

### Testing
- **Single crate test**: `cargo nextest run -p quickwit-search my_test_name`
- **Single test**: `cargo test -p quickwit-common my_test_name`
- **`make test-all`** — Starts Docker services (LocalStack S3, PostgreSQL, Pub/Sub emulator) and runs the full test suite with `cargo nextest run --all-features --retries 5`
- **`make test-failpoints`** — Runs failpoint tests only: `cargo nextest run --test failpoints --features fail/failpoints`
- Docker services: `make docker-compose-up` / `make docker-compose-down` (subset: `DOCKER_SER
```

</details>
