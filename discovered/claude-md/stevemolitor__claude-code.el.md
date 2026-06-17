---
name: stevemolitor__claude-code.el
source: https://github.com/stevemolitor/claude-code.el/blob/03199df8b3a1e9cd4857f0851f7a912ba524aff3/CLAUDE.md
repo: stevemolitor/claude-code.el
kind: claude-md
stars: 714
last_pushed: 2026-04-30T20:00:22Z
license: apache-2.0
score: 8
domains: [cli-tools, emacs-lisp]
tags: [emacs-lisp, coding-standards, build-system]
curated: 2026-06-15
curated_by: config-scout
---

# stevemolitor/claude-code.el — claude-md

**Why it's worth keeping:** It enforces strict naming conventions (prefixes), docstring formatting, and exact build targets that prevent an AI from deviating from project-specific Elisp standards.

**Summary:** This config provides highly specific structural and stylistic constraints for Emacs Lisp development.

**Source credibility:** High; the repository has significant star counts and recent maintenance activity.

**Recency:** Very current based on recent push history.

**Source:** [stevemolitor/claude-code.el/CLAUDE.md](https://github.com/stevemolitor/claude-code.el/blob/03199df8b3a1e9cd4857f0851f7a912ba524aff3/CLAUDE.md) · 714★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Code Development Guide

## Build and Test Commands
- Install package: `M-x package-install-file RET /path/to/claude-code.el`
- Use project Makefile targets (preferred methods):
  - Byte compile: `make compile`
  - Lint with checkdoc: `make checkdoc`
  - Run both checkdoc and compile: `make all`
- Alternative direct commands:
  - Byte compile: `emacs -Q --batch -f batch-byte-compile claude-code.el`
  - Check package: `emacs -Q --batch -l package-lint.el -f package-lint-batch-and-exit claude-code.el`
  - Lint with checkdoc: `emacs -Q --batch -l checkdoc -f checkdoc-file claude-code.el`

## Code Style Guidelines
- Prefix all functions/variables with `claude-code-` (public) or `claude-code--` (private)
- Follow standard Emacs Lisp naming conventions (kebab-case)
- Use lexical binding (include `lexical-binding: t` in header)
- Organize with section headers: `;;;; Section Name`
- Maintain proper package headers and autoload declarations
- Docstring for all functions and variables
  - Add a blank line after the first line of docstrings for multi-line descriptions
  - First line should be a complete sentence ending with a period
- Maintain dependency requirements: Emacs 30.1+, tra
```

</details>
