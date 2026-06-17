---
name: vega__vl-convert
source: https://github.com/vega/vl-convert/blob/0ad76bc54877a3e84960bab43a2c1477266d5dbe/CLAUDE.md
repo: vega/vl-convert
kind: claude-md
stars: 155
last_pushed: 2026-06-02T02:38:02Z
license: bsd-3-clause
score: 9
domains: [cli-tools, rust, python]
tags: [multi-language, system-constraints, dev-workflow]
curated: 2026-06-15
curated_by: config-scout
---

# vega/vl-convert — claude-md

**Why it's worth keeping:** The 'Critical Constraints' section is gold; it proactively prevents an agent from breaking the build by highlighting non-obvious requirements like single-threaded test execution and vendored JS dependencies.

**Summary:** Defines a multi-language architecture (Rust/Python) and provides a centralized command catalog via Pixi.

**Source credibility:** High; well-maintained, high-utility library with a clear, structured development workflow.

**Recency:** 

**Source:** [vega/vl-convert/CLAUDE.md](https://github.com/vega/vl-convert/blob/0ad76bc54877a3e84960bab43a2c1477266d5dbe/CLAUDE.md) · 155★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# vl-convert

Rust library + CLI + Python bindings for converting Vega-Lite to static images (SVG, PNG, PDF, JPEG) without internet.

## Architecture

```
vl-convert-rs/      Core Rust library (Deno v8 for JS execution)
vl-convert/         CLI wrapper
vl-convert-python/  Python bindings (PyO3/maturin)
vl-convert-vendor/  JS vendoring utility (dev only, not published)
```

## Development Environment

Uses **Pixi** for environment management. All commands via `pixi run <cmd>`.

## Essential Commands

```bash
pixi run dev-py         # Build Python lib in dev mode
pixi run test-rs        # Rust tests (single-threaded, Deno requirement)
pixi run test-cli       # CLI integration tests
pixi run test-py        # Python tests
pixi run fmt-rs         # Format Rust
pixi run fmt-py         # Format Python (Ruff)
pixi run clippy         # Lint Rust (warnings = errors)
pixi run vendor         # Regenerate vendored JavaScript
pixi run bundle-licenses # Bundle Rust licenses for Python wheels
```

## Code Quality

### Rust
- Format: `cargo fmt`
- Lint: clippy with `-D warnings` (no warnings allowed)
- Tests must be single-threaded: `cargo test -- --test-threads=1`

### Python
- Format + Lint: Ruff
```

</details>
