---
name: aallan__vera__skill
source: https://github.com/aallan/vera/blob/9eb700e0c0fcc32019355b1de17ca14dec2a3685/docs/SKILL.md
repo: aallan/vera
kind: skill
stars: 382
last_pushed: 2026-06-15T16:59:22Z
license: mit
score: 8
domains: [programming-languages, cli-tools, wasm]
tags: [language-spec, toolchain]
curated: 2026-06-16
curated_by: config-scout
---

# aallan/vera — skill

**Why it's worth keeping:** It includes critical 'anti-assumption' instructions for sandboxed environments and detailed behavioral differences between terminal and browser targets to prevent runtime errors.

**Summary:** A comprehensive technical reference for the Vera programming language, covering installation, full CLI toolchain, and execution nuances.

**Source credibility:** Strong; high star count (382) relative to niche language projects and very recent maintenance.

**Recency:** Current, aligned with modern development environments and Python/Node versions.

**Source:** [aallan/vera/docs/SKILL.md](https://github.com/aallan/vera/blob/9eb700e0c0fcc32019355b1de17ca14dec2a3685/docs/SKILL.md) · 382★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: vera-language
description: Write programs in the Vera programming language. Use when asked to write, edit, debug, or review Vera code (.vera files). Vera is a statically typed, purely functional language with algebraic effects, mandatory contracts, and typed slot references (@T.n) instead of variable names.
---

# Vera Language Reference

Vera is a programming language designed for LLMs to write. It uses typed slot references instead of variable names, requires contracts on every function, and makes all effects explicit.

## Installation

Vera requires Python 3.11 or later. Node.js 22+ is optional (only needed for `vera compile --target browser` and browser parity tests). Install from the repository:

```bash
git clone https://github.com/aallan/vera.git && cd vera
python -m venv .venv && source .venv/bin/activate
pip install -e .
```

This installs the `vera` command and all runtime dependencies (Lark parser, Z3 solver, wasmtime). For editor/agent integration via the Language Server Protocol, install the optional extra instead: `pip install -e ".[lsp]"` — see [LSP_SERVER.md](https://github.com/aallan/vera/blob/main/LSP_SERVER.md). After installation, verify it works:

```
```

</details>
