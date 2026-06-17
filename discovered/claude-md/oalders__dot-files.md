---
name: oalders__dot-files
source: https://github.com/oalders/dot-files/blob/a1581bad77d7b4eb4ec10d32448e0c511ea304c4/CLAUDE.md
repo: oalders/dot-files
kind: claude-md
stars: 29
last_pushed: 2026-06-13T15:42:22Z
license: unknown
score: 7
domains: [cli-tools, devops]
tags: [dotfiles, shell-scripting, automation]
curated: 2026-06-15
curated_by: config-scout
---

# oalders/dot-files — claude-md

**Why it's worth keeping:** Excellent use of 'Development Patterns' to explain non-obvious logic like the debouncing system and strict error handling (`set -eu -o pipefail`).

**Summary:** A comprehensive guide for a personal dotfiles repository covering installation orchestration, architecture, and specialized shell workflows.

**Source credibility:** Personal developer repository with moderate star count and high recent activity.

**Recency:** Current; reflects modern CLI toolings and dev workflows.

**Source:** [oalders/dot-files/CLAUDE.md](https://github.com/oalders/dot-files/blob/a1581bad77d7b4eb4ec10d32448e0c511ea304c4/CLAUDE.md) · 29★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a personal dotfiles repository containing configuration files, shell scripts, and automation tools for setting up development environments across macOS and Linux systems. The repository focuses on shell scripting, configuration management, and development tool setup.

## Key Commands

### Installation and Setup
- `./install.sh` - Main installation script that runs platform-specific and general installers
- `./installer/symlinks.sh` - Creates symbolic links for configuration files
- `./installer/homebrew.sh` - Installs Homebrew packages and casks (macOS)
- `./installer/npm.sh` - Installs Node.js packages
- `./installer/cpan.sh` - Installs Perl dependencies
- `./installer/cargo.sh` - Installs Rust packages

### Code Quality and Linting
- `precious tidy` - Auto-format shell scripts (shfmt) and Lua files (stylua)
- `precious lint` - Lint shell scripts and Lua files without modification
- `markdownlint-cli **/*.md` - Lint Markdown files
- `shfmt -w -s -i 4 **/*.sh` - Format shell scripts
- `stylua --check **/*.lua` - Check Lua formatting

#
```

</details>
