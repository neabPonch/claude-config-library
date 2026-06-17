---
name: colbsmcdolbs__magaziner
source: https://github.com/colbsmcdolbs/magaziner/blob/a9a2070d9665fa6f835aa971a8373a68de0bb070/CLAUDE.md
repo: colbsmcdolbs/magaziner
kind: claude-md
stars: 16
last_pushed: 2026-02-26T15:11:09Z
license: mit
score: 9
domains: [cli-tools, web-scraping, rust]
tags: [cargo, scraper, pipeline]
curated: 2026-06-16
curated_by: config-scout
---

# colbsmcdolbs/magaziner — claude-md

**Why it's worth keeping:** The architecture section is exceptionally useful because it explicitly lists CSS selectors and module responsibilities, preventing the AI from having to rediscover logic during scraping tasks. It also provides specific examples of how to run the CLI with varying flags.

**Summary:** Provides a comprehensive breakdown of a data-processing pipeline from fetching to EPUB generation.

**Source credibility:** Small project (16 stars) but high-quality, hand-written technical documentation.

**Recency:** Very current; follows modern Rust development and Claude Code interaction patterns.

**Source:** [colbsmcdolbs/magaziner/CLAUDE.md](https://github.com/colbsmcdolbs/magaziner/blob/a9a2070d9665fa6f835aa971a8373a68de0bb070/CLAUDE.md) · 16★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

```bash
# Build
cargo build

# Build release binary
cargo build --release

# Run
cargo run -- --url https://www.lrb.co.uk/the-paper/v47/n06

# Run with options
cargo run -- --url <URL> --output ./downloads --delay 1000 --force

# Run all tests
cargo test

# Run a single test
cargo test test_extract_article_links_from_issue
cargo test test_valid_lrb_url_should_pass

# Lint
cargo clippy
```

## Architecture

`magaziner` is a CLI tool that downloads a London Review of Books (LRB) issue and generates an EPUB file from it.

**Pipeline (orchestrated in `main.rs`):**
1. Fetch the issue page HTML (`fetch.rs`)
2. Parse article links, title, CSS, and cover image URI from the issue page (`parser.rs`)
3. Fetch each article page and extract its title and body HTML (`parser.rs`)
4. Build and write an EPUB file (`epub.rs`)

**Modules:**
- `main.rs` — CLI args via `clap` (derive), orchestrates the pipeline, manages output path and `--force` flag
- `fetch.rs` — blocking HTTP requests via `reqwest`; applies the configurable delay before each fetch to rate-limit requests
-
```

</details>
