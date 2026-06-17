---
name: asdf-community__asdf-zig
source: https://github.com/asdf-community/asdf-zig/blob/bf29a9b2671d3adc5cb7d95a3303b764f46044d7/CLAUDE.md
repo: asdf-community/asdf-zig
kind: claude-md
stars: 80
last_pushed: 2026-04-30T08:24:58Z
license: apache-2.0
score: 8
domains: [cli-tools, devops]
tags: [shell, python, asdf, zig]
curated: 2026-06-15
curated_by: config-scout
---

# asdf-community/asdf-zig — claude-md

**Why it's worth keeping:** The 'Code Architecture' section explains the operational sequence (download/verification) rather than just file locations. It also includes specific style rules and environment variables essential for maintaining tool consistency.

**Summary:** A concise guide to an asdf plugin that details functional logic flows, command-line tools, and environment variables.

**Source credibility:** High; part of a recognized community toolset with recent maintenance.

**Recency:** Current; specifically mentions Claude Code and uses modern linting standards.

**Source:** [asdf-community/asdf-zig/CLAUDE.md](https://github.com/asdf-community/asdf-zig/blob/bf29a9b2671d3adc5cb7d95a3303b764f46044d7/CLAUDE.md) · 80★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is an [asdf](https://asdf-vm.com) plugin for managing [Zig](https://ziglang.org/) installations. It also supports installing [ZLS](https://github.com/zigtools/zls) (Zig Language Server) alongside Zig for IDE support.

## Code Architecture

The plugin follows the asdf plugin convention with scripts in `bin/` and shared logic in `lib/`:

- **`bin/`**: Entry points called by asdf (download, install, list-all, latest-stable)
- **`lib/utils.py`**: Core Python logic for fetching the Zig version index, resolving platform-specific download URLs, and downloading tarballs with SHA256 verification
- **`lib/commands/`**: Additional asdf subcommands (mirror management)

The download flow:
1. `bin/download` calls `lib/utils.py download` which fetches from ziglang.org/download/index.json
2. Tries community mirrors (randomized order) before falling back to official source
3. Downloads both Zig and ZLS tarballs, verifies SHA256 checksums
4. `bin/install` extracts and places binaries in the asdf install path

## Common Commands

```bash
# Format shell scripts
```

</details>
