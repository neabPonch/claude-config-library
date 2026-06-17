---
name: janreges__siteone-crawler
source: https://github.com/janreges/siteone-crawler/blob/63203298f00e97b5e07525a9b7c40216f4f394f7/CLAUDE.md
repo: janreges/siteone-crawler
kind: claude-md
stars: 770
last_pushed: 2026-03-30T00:33:57Z
license: mit
score: 9
domains: [cli-tools, web-crawling, rust]
tags: [architecture-heavy, lifecycle-driven, system-design]
curated: 2026-06-15
curated_by: config-scout
---

# janreges/siteone-crawler — claude-md

**Why it's worth keeping:** The step-by-step 'Crawl Lifecycle' and specific detail on traits/concurrency primitives create a perfect mental model for an AI to navigate complex state changes.

**Summary:** Provides an exhaustive architectural breakdown of the crawler's exact execution lifecycle, component interactions, and concurrency model.

**Source credibility:** High; the repository has significant stars (770) indicating a mature, well-tested tool.

**Recency:** Current; explicitly references Claude Code and follows modern Rust development patterns.

**Source:** [janreges/siteone-crawler/CLAUDE.md](https://github.com/janreges/siteone-crawler/blob/63203298f00e97b5e07525a9b7c40216f4f394f7/CLAUDE.md) · 770★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Setup After Clone

```bash
git config core.hooksPath .githooks               # enable pre-commit hook (fmt + clippy + tests)
```

## Build & Test Commands

```bash
cargo fmt                                         # auto-format code (always run before build)
cargo build                                       # debug build
cargo build --release                             # release build (~11s)
cargo test                                        # unit tests + offline integration tests (~300 tests)
cargo test --test integration_crawl -- --ignored --test-threads=1  # network integration tests (crawls crawler.siteone.io)
cargo test scoring::ci_gate::tests::all_checks_pass  # run a single test by name
cargo clippy -- -D warnings                       # lint (CI enforces zero warnings)
cargo fmt -- --check                              # format check
```

## Quick Run

```bash
./target/release/siteone-crawler --url=https://example.com --single-page
./target/release/siteone-crawler --url=https://example.com --output=json --http-cache-dir=  # no cache
./target/release/siteon
```

</details>
