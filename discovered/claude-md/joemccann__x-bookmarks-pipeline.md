---
name: joemccann__x-bookmarks-pipeline
source: https://github.com/joemccann/x-bookmarks-pipeline/blob/19f4d709a41c4cabd866c34f6cde3d52ca279bb4/CLAUDE.md
repo: joemccann/x-bookmarks-pipeline
kind: claude-md
stars: 93
last_pushed: 2026-03-20T03:48:47Z
license: mit
score: 9
domains: [cli-tools, rust, automation, data-pipeline]
tags: [architecture-map, environment-specs, error-handling-patterns]
curated: 2026-06-16
curated_by: config-scout
---

# joemccann/x-bookmarks-pipeline — claude-md

**Why it's worth keeping:** It maps specific modules to their exact responsibilities and documents complex side-effect logic (like the CDP browser flow) that prevents breaking changes. It also details error-handling/resilience patterns, allowing Claude to write code consistent with existing recovery logic.

**Summary:** A highly detailed architectural and operational guide for a Rust-based automation pipeline.

**Source credibility:** The repository has healthy star counts and high-quality, highly specific technical documentation.

**Recency:** Very current; includes recent pricing data and modern Pine Script versions.

**Source:** [joemccann/x-bookmarks-pipeline/CLAUDE.md](https://github.com/joemccann/x-bookmarks-pipeline/blob/19f4d709a41c4cabd866c34f6cde3d52ca279bb4/CLAUDE.md) · 93★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## Rust-only architecture

This repository is a Rust implementation of the X bookmark pipeline with shared provider abstractions and a single executable workflow in `src/main.rs`.

- `llm.rs` exposes the shared `LLMProvider` trait (`classify`, `analyze_image`, `generate_code`) and provider wrappers.
- `cache.rs` owns SQLite persistence with shared mutable access using `Arc<Mutex<Connection>>`.
- `orchestrator.rs` coordinates bounded worker parallelism and `on_meta_saved` side effects.
- `notify.rs` implements `SmtpNotifier` via `lettre`; one email per cycle listing new bookmarks only.
- `error.rs` centralizes `PipelineError` and conversion of external failures.
- `browser.rs` implements CDP auto-consent (connects to existing Chrome via HTTP discovery on port 9222), and closes only the OAuth callback tab after auth by exact redirect URI match.
- `cost.rs` tracks per-bookmark LLM token usage and USD costs with per-provider pricing.
- `x_api_cache.rs` caches username→user_id mappings, token validation state, and tracks X API request budgets.
- `main.rs` handles startup, env loading, provider bootstrap, and CLI dispatch.

## Setup

```bash
cp .env.example .env
cargo build
```

</details>
