---
name: jackfranklin__dotfiles
source: https://github.com/jackfranklin/dotfiles/blob/3f3205e769ec3f5c80feaad856dcfb012e426b95/CLAUDE.md
repo: jackfranklin/dotfiles
kind: claude-md
stars: 250
last_pushed: 2026-06-12T15:09:54Z
license: mit
score: 9
domains: [cli-tools, dev-environment]
tags: [dotfiles, neovim, shell, makefile]
curated: 2026-06-16
curated_by: config-scout
---

# jackfranklin/dotfiles — claude-md

**Why it's worth keeping:** Provides deep architectural context for nested configuration hierarchies (Neovim Lua modules) and explicit deployment mechanics through Makefile targets. This prevents an AI from breaking machine-specific overrides or mismanaging symlinks.

**Summary:** Detailed guide for managing a symlink-based dotfiles environment via Makefiles, covering complex Neovim architecture and shell workflows.

**Source credibility:** High; highly-starred, active personal developer environment.

**Recency:** Very current, featuring dedicated Claude Code integration instructions.

**Source:** [jackfranklin/dotfiles/CLAUDE.md](https://github.com/jackfranklin/dotfiles/blob/3f3205e769ec3f5c80feaad856dcfb012e426b95/CLAUDE.md) · 250★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

Personal dotfiles for Jack Franklin. Uses a **symlink-based installation** strategy: files are stored in this repo without a leading dot, then symlinked into place with `make <target>`. No `stow` — the Makefile manages all symlinks explicitly.

## Common Commands

```bash
# Run Lua unit tests (requires busted)
make lua_specs

# Install individual tool configs (creates symlinks)
make neovim      # ~/dotfiles/nvim → ~/.config/nvim
make fish        # ~/dotfiles/fish → ~/.config/fish
make git         # gitconfig + gitignore_global → ~/.gitconfig / ~/.gitignore_global
make kitty       # ~/dotfiles/kitty → ~/.config/kitty
make claude      # settings.json + CLAUDE.md + skills → ~/.claude/

# Install system packages (Ubuntu/Debian)
make ubuntu-deps

# Install global npm language servers (TypeScript, Svelte, ESLint, etc.)
make language_servers_global
```

## Architecture

### Installation Model

Each `make` target runs `ln -nsf` to create a symlink. There is no automatic install — targets must be run individually. The `DIR` variable defaults to `~/dotfiles`.

###
```

</details>
