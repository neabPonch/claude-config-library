---
name: yqrashawn__yqdotfiles
source: https://github.com/yqrashawn/yqdotfiles/blob/ed4627bdcabec0946245df9019a25acd41ecbb84/CLAUDE.md
repo: yqrashawn/yqdotfiles
kind: claude-md
stars: 79
last_pushed: 2026-06-15T04:56:03Z
license: mit
score: 8
domains: [editors, development-workflows]
tags: [emacs, elisp, doom-emacs, workflow]
curated: 2026-06-15
curated_by: config-scout
---

# yqrashawn/yqdotfiles — claude-md

**Why it's worth keeping:** It captures essential REPL-driven development steps—like evaluating buffers after changes and loading test files before running them—that an LLM would otherwise overlook.

**Summary:** Provides procedural guidance for maintaining a Doom Emacs configuration, focusing on buffer evaluation and test execution workflows.

**Source credibility:** High-quality personal dotfiles with recent activity and consistent maintenance.

**Recency:** Current; includes modern workflow patterns like MCP server integration and tool-specific instructions.

**Source:** [yqrashawn/yqdotfiles/CLAUDE.md](https://github.com/yqrashawn/yqdotfiles/blob/ed4627bdcabec0946245df9019a25acd41ecbb84/CLAUDE.md) · 79★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to LLM when working with code in `<project-root>/.doom.d` in this repository.

## Doom Emacs Configuration (.doom.d/)

The `.doom.d/` directory contains a comprehensive Doom Emacs configuration with extensive customizations:

### Instructions
- use `get_buffer_file_path` tool to get absolute path of a buffer
- whenever working on emacs lisp buffer `foo.el`, evaluate the buffer after changes made, check `foo-test.el` at the same directory see if corresponding test is missing or outdated

### Run Tests
- use run ert test tool to run elisp ert tests
- evaluate test file before run the test, test files are not loaded by default

### Core Files
- **init.el**: Doom module configuration and feature flags
- **config.el**: Main configuration with fonts, themes, and personal settings
- **packages.el**: Additional package declarations and overrides

### Language-Specific Configurations
- **clojure.el**: Clojure/ClojureScript development setup
- **js.el**: JavaScript/TypeScript configuration
- **golang.el**: Go language support
- **lisp.el** / **clisp.el**: Common Lisp development
- **lang.el**: General language configurations

### Feature Modules
- **g
```

</details>
