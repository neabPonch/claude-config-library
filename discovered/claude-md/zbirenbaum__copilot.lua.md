---
name: zbirenbaum__copilot.lua
source: https://github.com/zbirenbaum/copilot.lua/blob/b54c05349d406f7af11b150824efa8e4f90015c6/CLAUDE.md
repo: zbirenbaum/copilot.lua
kind: claude-md
stars: 4086
last_pushed: 2026-06-13T02:34:23Z
license: mit
score: 9
domains: [cli-tools, neovim-plugin, lua]
tags: [architecture-map, dev-workflow, neovim]
curated: 2026-06-16
curated_by: config-scout
---

# zbirenbaum/copilot.lua — claude-md

**Why it's worth keeping:** The sequence-based initialization flow and module-to-role table are perfect for helping an LLM navigate codebase dependencies. Explicitly defining design patterns (like coroutine-based async) prevents the AI from suggesting incompatible logic.

**Summary:** Provides a high-density technical map of the plugin's architecture and development lifecycle. It bridges the gap between 'what the code is' and 'how it works internally'.

**Source credibility:** High; a popular, well-maintained Neovim plugin with significant community adoption.

**Recency:** Very recent; includes up-to-date requirements for Neovim and Node.js.

**Source:** [zbirenbaum/copilot.lua/CLAUDE.md](https://github.com/zbirenbaum/copilot.lua/blob/b54c05349d406f7af11b150824efa8e4f90015c6/CLAUDE.md) · 4086★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

copilot.lua is a pure Lua Neovim plugin for GitHub Copilot integration, replacing github/copilot.vim. It communicates with the Copilot Language Server via Neovim's built-in LSP client to provide inline suggestions, a completion panel, and next-edit suggestions (NES).

**Requirements**: Neovim 0.11+, Node.js 22+ (for the default nodejs server mode).

## Development Commands

```bash
make deps                          # Clone mini.nvim and osv into deps/
make test                          # Run all tests (auto-fetches deps)
make test_file FILE=tests/test_client.lua  # Run a single test file
```

**Code quality** (checked in CI):
- **Format**: Stylua (config in `.stylua.toml`)
- **Lint**: Luacheck (config in `.luacheckrc`, vim globals allowed)
- **Typecheck**: Lua type annotations

## Architecture

### Initialization Flow

`plugin/copilot.lua` registers the `:Copilot` user command. When `require("copilot").setup(opts)` is called:

1. Validates Neovim version, sets up highlights, merges config
2. On `:Copilot` or lazy trigger → `client.setup()` start
```

</details>
