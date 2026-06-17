---
name: jakewvincent__texmagic.nvim
source: https://github.com/jakewvincent/texmagic.nvim/blob/8172d2d974b444dcc996d87a9e05723348676d5e/CLAUDE.md
repo: jakewvincent/texmagic.nvim
kind: claude-md
stars: 58
last_pushed: 2026-03-02T15:10:15Z
license: gpl-3.0
score: 8
domains: [cli-tools, editors]
tags: [neovim, lua, plugin-architecture]
curated: 2026-06-16
curated_by: config-scout
---

# jakewvincent/texmagic.nvim — claude-md

**Why it's worth keeping:** It documents crucial implementation constraints (like disk vs buffer reading) and lists specific diagnostic commands for verification without a test suite.

**Summary:** Provides a detailed architectural map of a Neovim plugin, including functional breakdowns and integration patterns.

**Source credibility:** A stable niche Neovim plugin with reasonable social proof and recent updates.

**Recency:** Current; highly applicable to the current capabilities of Claude Code's repository understanding.

**Source:** [jakewvincent/texmagic.nvim/CLAUDE.md](https://github.com/jakewvincent/texmagic.nvim/blob/8172d2d974b444dcc996d87a9e05723348676d5e/CLAUDE.md) · 58★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

TeXMagic.nvim is a Neovim plugin that selects LaTeX build engines based on magic comments (`%! TEX program = xelatex`) at the top of `.tex` files. It's designed to integrate with the TexLab LSP server via nvim-lspconfig, enabling per-project build engine configuration.

## Development

There is no build system, test suite, or linter configured. The plugin is pure Lua + VimScript and is tested manually in Neovim. To test changes, load the plugin in Neovim (e.g. via a plugin manager pointing to the local path) and open a `.tex` file with magic comments.

Diagnostic commands available in Neovim: `:TeXMagicShowComments`, `:TeXMagicCommentsFound`, `:TeXMagicSetupStatus`, `:TeXMagicSelectedProgram`, `:TeXMagicConfigFound`, `:TeXMagicLoaded`.

## Architecture

All core logic lives in `lua/texmagic/magiccomments.lua`. The module `lua/texmagic/init.lua` simply re-exports it.

### magiccomments.lua — the entire plugin logic

- `M.findMagicComments(path)` — reads a file from disk via `io.open`, collects consecutive lines from the top matching the pattern `%
```

</details>
