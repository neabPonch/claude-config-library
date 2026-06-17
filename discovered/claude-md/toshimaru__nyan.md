---
name: toshimaru__nyan
source: https://github.com/toshimaru/nyan/blob/543da7b6d7cf8a9fb8935d0863274fa673212d09/CLAUDE.md
repo: toshimaru/nyan
kind: claude-md
stars: 230
last_pushed: 2026-06-04T00:10:47Z
license: mit
score: 8
domains: [cli-tools, go]
tags: [go, cobra, syntax-highlighting]
curated: 2026-06-14
curated_by: config-scout
---

# toshimaru/nyan — claude-md

**Why it's worth keeping:** The inclusion of 'Test output' examples and the detailed explanation of the theme registry pattern allows an agent to extend the project effectively without manual exploration.

**Summary:** Provides clear architecture mappings and specific command-line execution patterns for a Go CLI tool.

**Source credibility:** Strong; 230 stars indicates a popular, well-regarded open source utility with recent maintenance.

**Recency:** Current; follows standard Go project conventions compatible with Claude Code workflows.

**Source:** [toshimaru/nyan/CLAUDE.md](https://github.com/toshimaru/nyan/blob/543da7b6d7cf8a9fb8935d0863274fa673212d09/CLAUDE.md) · 230★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

`nyan` is a Go CLI tool that provides syntax-highlighted output for files, similar to `cat` but with colorization. It's named after Nyan Cat and uses the Chroma syntax highlighting library.

## Architecture

- **Entry point**: `main.go` - Simple wrapper that calls `cmd.Execute()`
- **CLI logic**: `cmd/root.go` - Contains all command logic using Cobra framework
- **Syntax highlighting**: Uses `github.com/alecthomas/chroma/v2` for tokenization and formatting
- **Themes**: Custom theme registry in `styles/` directory with individual theme files
- **Core functionality**: 
  - File reading with automatic language detection via Chroma's lexers
  - Terminal detection for conditional colorization
  - Line numbering support via custom `numberWriter`
  - Theme switching and listing capabilities

## Development Commands

### Build and Test
```bash
go build -v
go test ./...
```

### Run locally
```bash
go run main.go [flags] FILE
```

### Test output
```bash
# Normal output test
go run main.go -- main.go

# Test with different themes
go run main.go -t dracul
```

</details>
