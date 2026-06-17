---
name: NihilDigit__renpak
source: https://github.com/NihilDigit/renpak/blob/42a4d0cdc02957c97b01eb0b3df265d28ee33491/CLAUDE.md
repo: NihilDigit/renpak
kind: claude-md
stars: 5
last_pushed: 2026-03-17T16:25:43Z
license: mpl-2.0
score: 9
domains: [cli-tools, systems-programming, game-dev]
tags: [rust, python-ffi, compression, low-level]
curated: 2026-06-15
curated_by: config-scout
---

# NihilDigit/renpak — claude-md

**Why it's worth keeping:** It uses highly specific 'Do Not' lists to prevent common architectural blunders like using PyO3 instead of ctypes or assuming available system disk space. The technical constraints provide essential guardrails for maintaining low-level compatibility with a specific engine's environment.

**Summary:** A high-density technical spec for a Rust/Python bridge toolchain designed specifically for the Ren'Py game engine. It covers architecture, strict FFI requirements, and critical runtime constraints.

**Source credibility:** The repo has 5 stars and was updated very recently (3 months ago), suggesting active maintenance.

**Recency:** Extremely current; relevant to modern Rust and Python interoperability patterns.

**Source:** [NihilDigit/renpak/CLAUDE.md](https://github.com/NihilDigit/renpak/blob/42a4d0cdc02957c97b01eb0b3df265d28ee33491/CLAUDE.md) · 5★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# renpak

AVIF compression toolchain for Ren'Py games.
Rust CLI with interactive TUI + runtime Ren'Py plugin.

License: MPL-2.0

## Architecture

Two Rust crates + runtime plugin:

- `crates/renpak-core/` — Build engine: RPA read/write, AVIF/AVIS encoding, parallel pipeline, CLI, TUI
- `crates/renpak-rt/` — Runtime decoder: AVIS frame-level random access, exports extern "C" API for ctypes
- `python/runtime/` — Deployed to game `game/` directory (.rpy + .py)
- `install.sh` — Builds and symlinks `renpak` binary to ~/.local/bin/

## Build

```bash
cargo build --release
```

Static linking for distribution (used by CI):

```bash
RENPAK_STATIC=1 cargo build --release
```

## Technical Constraints

### Ren'Py Runtime Environment

- Runtime plugin runs on Ren'Py's bundled Python (2.7 for Ren'Py 7.x, 3.9 for 8.x), not system Python
- Native libraries loaded via ctypes.CDLL — must export pure C ABI (extern "C"), no PyO3
- Runtime Python code cannot depend on any third-party packages — stdlib + Ren'Py builtins only
- Ren'Py's image preloader runs on background threads — Rust decoder must be thread-safe (per-thread context, no global state)

### Encoding Constraints

- AVIF color space: must
```

</details>
