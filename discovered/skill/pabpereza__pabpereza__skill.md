---
name: pabpereza__pabpereza__skill
source: https://github.com/pabpereza/pabpereza/blob/ffd5fb07973a8722d07ed98d381cdea81c558a59/.claude/skills/neovim/SKILL.md
repo: pabpereza/pabpereza
kind: skill
stars: 430
last_pushed: 2026-06-15T01:28:00Z
license: apache-2.0
score: 9
domains: [cli-tools, editor-config]
tags: [neovim, lua, lsp, devtools]
curated: 2026-06-15
curated_by: config-scout
---

# pabpereza/pabpereza — skill

**Why it's worth keeping:** Provides clear architectural hierarchy, standardized module patterns (M.setup), and explicit loading strategy tables that allow an agent to extend the config without breaking it.

**Summary:** A highly structured technical manual for a modular Lua-based Neovim configuration.

**Source credibility:** High-quality personal configuration with strong community validation (430 stars).

**Recency:** Extremely current, utilizing modern tools like lazy.nvim and blink.cmp.

**Source:** [pabpereza/pabpereza/.claude/skills/neovim/SKILL.md](https://github.com/pabpereza/pabpereza/blob/ffd5fb07973a8722d07ed98d381cdea81c558a59/.claude/skills/neovim/SKILL.md) · 430★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: neovim
description: Comprehensive guide for this Neovim configuration - a modular, performance-optimized Lua-based IDE. Use when configuring plugins, adding keybindings, setting up LSP servers, debugging, or extending the configuration. Covers lazy.nvim, 82+ plugins across 9 categories, DAP debugging, AI integrations, and performance optimization.
---

# Neovim Configuration Skill

A comprehensive guide for working with this modular, performance-optimized Neovim configuration built on lazy.nvim.

## Quick Reference

| Metric | Value |
|--------|-------|
| Plugin Manager | lazy.nvim |
| Total Plugins | 82 |
| Target Startup | <50ms |
| Module Pattern | `M.setup()` |
| Leader Key | `<Space>` |

## Architecture Overview

```
~/.config/nvim/
├── init.lua                  # Entry point
├── lua/
│   ├── config/               # Core configuration (11 modules)
│   │   ├── lazy.lua          # Plugin manager bootstrap
│   │   ├── options.lua       # Vim options
│   │   ├── keymaps.lua       # Key bindings
│   │   ├── autocmds.lua      # Autocommands
│   │   └── performance.lua   # Startup optimization
│   ├── plugins/specs/        # Plugin specs (9 categories)
│   │   ├── core.lua
```

</details>
