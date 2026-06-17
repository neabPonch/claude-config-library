---
name: tracyone__vinux
source: https://github.com/tracyone/vinux/blob/e311f59227edd844b875a78405de1d73f5b25b7b/CLAUDE.md
repo: tracyone/vinux
kind: claude-md
stars: 250
last_pushed: 2026-05-09T15:13:41Z
license: mit
score: 9
domains: [cli-tools, editors]
tags: [vim, neovim, dotfiles, modular]
curated: 2026-06-15
curated_by: config-scout
---

# tracyone/vinux — claude-md

**Why it's worth keeping:** Uses structured tables to map function modules to purposes and explicitly defines the project's custom feature-toggle system to prevent breaking core logic.

**Summary:** A highly detailed guide for a modular Vim/Neovim configuration that explains unique internal logic and tool commands.

**Source credibility:** High; it is a popular (250 stars) and actively maintained dotfile repository.

**Recency:** Recent, reflecting modern Neovim/LSP workflows.

**Source:** [tracyone/vinux/CLAUDE.md](https://github.com/tracyone/vinux/blob/e311f59227edd844b875a78405de1d73f5b25b7b/CLAUDE.md) · 250★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Common Commands
- **Install / bootstrap** – Run the shell script that sets up Vim/Neovim and installs plugins.
  ```bash
  bash install.sh
  ```
- **Update plugins** – Refresh all vim‑plug plugins.
  ```bash
  vim +PlugUpdate +qall   # for Vim
  nvim +PlugUpdate +qall  # for Neovim
  ```
- **Open Vim/Neovim** – Start the editor with the current configuration.
  ```bash
  vim      # or nvim
  ```
- **Generate unit tests** – In Vim, the `:GenerateTest` command (provided by `rc/vim-ai.vim`) can create test stubs for a selected code block.
- **Run LSP diagnostics** – Use Neovim's built‑in LSP client (configured via `lua/nvim_lsp.lua`).
- **Install language servers** – Via Mason: `MasonInstall <server>`.
- **Feature management**:
  - `:call te#feat#feat_dyn_enable(1)` - Enable a feature
  - `:call te#feat#feat_dyn_enable(0)` - Disable a feature
  - `<Leader>fe` - Enable feature interactively
  - `<Leader>fd` - Disable feature interactively

## High‑Level Architecture

### Overview
The repository is a **Vim/Neovim configuration** named *vinux* - a highly modular, cross-
```

</details>
