---
name: jwiegley__dot-emacs__claude
source: https://github.com/jwiegley/dot-emacs/blob/189f30a0e2d06ce93bd3bc36c83c7beb0a877301/lisp/CLAUDE.md
repo: jwiegley/dot-emacs
kind: claude-md
stars: 782
last_pushed: 2026-06-10T18:29:44Z
license: unknown
score: 9
domains: [cli-tools, development-environment, emacs-lisp]
tags: [elisp, build-systems, testing, coding-standards]
curated: 2026-06-15
curated_by: config-scout
---

# jwiegley/dot-emacs — claude-md

**Why it's worth keeping:** It provides exact CLI command patterns for multiple build tools (Eask, Make, Cask) and strict naming conventions to ensure AI-generated code fits the existing namespace.

**Summary:** A high-density guide for Emacs Lisp development that covers build systems, testing workflows, and specific coding standards.

**Source credibility:** Extremely high; John Wiegley is a prominent Emacs contributor with a highly active, heavily starred repository.

**Recency:** Very current; incorporates modern protocols like MCP and latest Elisp practices.

**Source:** [jwiegley/dot-emacs/lisp/CLAUDE.md](https://github.com/jwiegley/dot-emacs/blob/189f30a0e2d06ce93bd3bc36c83c7beb0a877301/lisp/CLAUDE.md) · 782★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is John Wiegley's Emacs Lisp personal configuration and packages repository. It contains custom Emacs modules, packages, and configurations organized as a collection of independent Elisp projects.

## Key Packages and Modules

The repository contains several major components:

- **Core Modules**: Individual `.el` files in the root directory (e.g., `cl-info.el`, `org-config.el`, `gptel-presets.el`)
- **Packages with Subdirectories**: Larger packages with their own structure (e.g., `chess/`, `use-package/`, `async/`, `gptel/`)
- **MCP Integration**: Model Context Protocol server library (`mcp-server-lib/`) and related tools
- **Org-mode Extensions**: Various org-mode enhancements (`org-roam-ext.el`, `org-ql-ext.el`, `org-smart-capture.el`)

## Emacs Lisp Development Patterns

### Code Organization

**Lexical Binding** - All modern packages use lexical binding:
```elisp
;;; package-name.el --- Description -*- lexical-binding: t; -*-
```

**File Structure** - Standard Elisp package layout:
```elisp
;;; package-name.el --- Brief description -*
```

</details>
