---
name: bennigo__dotfiles__claude
source: https://github.com/bennigo/dotfiles/blob/621049315e8ac995b012205f4c96ffbd8a7b49e6/neovim/.config/nvim/CLAUDE.md
repo: bennigo/dotfiles
kind: claude-md
stars: 0
last_pushed: 2026-06-15T09:01:42Z
license: unknown
score: 9
domains: [cli-tools, dev-environment, ai-agents]
tags: [neovim, dotfiles, workflow-automation]
curated: 2026-06-15
curated_by: config-scout
---

# bennigo/dotfiles — claude-md

**Why it's worth keeping:** It uses an 'Environment Map' pattern that defines specific keybindings for tool interactions and establishes clear architectural rules (e.g., extension patterns) to prevent the AI from breaking local configurations.

**Summary:** A comprehensive architectural map of a Neovim development environment, detailing a hierarchy of AI agents and specialized tool integrations.

**Source credibility:** High-density personal dotfile configuration with expert-level Neovim knowledge.

**Recency:** Extremely current; references latest Neovim versions and Claude Code CLI integrations.

**Source:** [bennigo/dotfiles/neovim/.config/nvim/CLAUDE.md](https://github.com/bennigo/dotfiles/blob/621049315e8ac995b012205f4c96ffbd8a7b49e6/neovim/.config/nvim/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Neovim Configuration - LazyVim-based IDE

This file provides context for Claude Code when working with this Neovim configuration.

## Overview

**Editor**: Neovim v0.11.4 (built from source, RelWithDebInfo)
**Foundation**: LazyVim with extensive customization
**Multi-language**: Python, R, LaTeX, Lua, Markdown, C/C++
**Key Integrations**: Claude Code, PostgreSQL Database UI, Obsidian, R Statistical Computing

This is a production IDE for scientific computing (GPS/GNSS data processing), knowledge management (Obsidian), and multi-language development.

## Critical Integrations

### Claude Code (AI Pair Programming - Primary)

**File**: `lua/plugins/claude-code.lua`
**Primary Keymap**: `<M-c>` (toggle/focus)
**Leader Mappings**: `<leader>aci` (toggle), `<leader>acc` (focus), `<leader>acs` (send), `<leader>acd/D` (accept/reject diff), `<leader>acR` (remote control)

**Configuration**:
- Floating window: 95% width, 95% height
- Diff: vertical split, keeps terminal focus
- Auto-close diffs on accept
- WebSocket connection to Claude Code CLI
- Transparency enabled (winblend: 30)
- Remote control: `<leader>acR` opens Claude Code with `--remote-control` flag, accessible from phone/browser
```

</details>
