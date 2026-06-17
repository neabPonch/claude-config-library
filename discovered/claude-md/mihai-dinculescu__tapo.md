---
name: mihai-dinculescu__tapo
source: https://github.com/mihai-dinculescu/tapo/blob/ee6dafce59a06383a85c7a70e08c9415642a6f79/CLAUDE.md
repo: mihai-dinculescu/tapo
kind: claude-md
stars: 766
last_pushed: 2026-06-12T21:22:57Z
license: mit
score: 8
domains: [rust, python, systems-programming]
tags: [pyo3, rust, interop, bindings]
curated: 2026-06-14
curated_by: config-scout
---

# mihai-dinculescu/tapo — claude-md

**Why it's worth keeping:** It contains highly specific, non-obvious instructions for PyO3 type conversion and Python stub conventions that prevent breaking changes. This encodes 'tribal knowledge' regarding edge cases in Rust-to-Python interoperability.

**Summary:** Defines the architecture for a multi-crate Rust/Python project and provides strict rules for maintaining cross-language bindings.

**Source credibility:** The source is a high-quality, actively maintained Rust project with significant community interest (766 stars).

**Recency:** Current; it includes modern context such as MCP server integration.

**Source:** [mihai-dinculescu/tapo/CLAUDE.md](https://github.com/mihai-dinculescu/tapo/blob/ee6dafce59a06383a85c7a70e08c9415642a6f79/CLAUDE.md) · 766★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Architecture

### Workspace Members
- **`tapo`** — Core Rust library (published to crates.io)
- **`tapo-py`** — Python bindings via PyO3/maturin (published to PyPI)
- **`tapo-mcp`** — MCP server exposing Tapo devices as AI tools/resources

## Cross-Language Bindings

When modifying Rust code that has Python bindings (tapo-py), always check if corresponding Python type stubs (.pyi files) need updating. The `debug` feature in `tapo` is **user-facing public API** — `tapo-py` enables it (`features = ["python", "debug"]`), so all `debug`-gated types are also exposed to Python. Treat changes behind `cfg(feature = "debug")` as public API changes requiring changelog entries for both Rust and Python.

### Exposing Rust Types to Python
- **Simple value/result types**: Annotate directly in the `tapo` crate with `#[cfg_attr(feature = "python", pyo3::prelude::pyclass(from_py_object, ...))]` and `#[cfg(feature = "python")] crate::impl_to_dict!(TypeName);`. Do NOT create a redundant wrapper struct in `tapo-py`.
- **`serde_json::Value` → Python**: Use `crate::python::serde_object
```

</details>
