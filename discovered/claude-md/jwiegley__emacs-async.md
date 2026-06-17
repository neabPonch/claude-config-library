---
name: jwiegley__emacs-async
source: https://github.com/jwiegley/emacs-async/blob/5faab28916603bb324d9faba057021ce028ca847/CLAUDE.md
repo: jwiegley/emacs-async
kind: claude-md
stars: 911
last_pushed: 2026-03-18T18:03:37Z
license: gpl-3.0
score: 8
domains: [emacs-lisp, cli-tools]
tags: [build-automation, architectural-patterns, implementation-details]
curated: 2026-06-15
curated_by: config-scout
---

# jwiegley/emacs-async — claude-md

**Why it's worth keeping:** The 'Key Implementation Details' section offers high-value technical constraints that prevent logic errors in inter-process communication and variable injection.

**Summary:** Provides architectural context, vital build/test commands, and technical implementation details specific to the library's async mechanism.

**Source credibility:** High; a well-starred (911) and recently maintained Emacs utility.

**Recency:** Current; demonstrates modern project-specific guidance patterns for AI agents.

**Source:** [jwiegley/emacs-async/CLAUDE.md](https://github.com/jwiegley/emacs-async/blob/5faab28916603bb324d9faba057021ce028ca847/CLAUDE.md) · 911★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

emacs-async is an Emacs Lisp library that provides asynchronous processing capabilities in Emacs. It allows running elisp code in subprocess Emacs instances to avoid blocking the main Emacs session.

## Architecture

The library consists of several modules:

- **async.el**: Core async functionality - provides `async-start`, `async-start-process`, and related functions for running code asynchronously
- **dired-async.el**: Asynchronous file operations for Dired (copy, rename, symlink)
- **async-bytecomp.el**: Asynchronous byte compilation of packages
- **async-package.el**: Asynchronous package installation/upgrades
- **smtpmail-async.el**: Send emails asynchronously via SMTP

The core mechanism works by starting a child Emacs process with minimal initialization, injecting required variables from parent, executing the provided code, and returning results via process communication.

## Development Commands

```bash
# Build and compile
make all                    # Clean, generate autoloads, and compile all .el files
make compile               # Compile indi
```

</details>
