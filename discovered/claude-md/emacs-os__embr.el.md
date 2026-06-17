---
name: emacs-os__embr.el
source: https://github.com/emacs-os/embr.el/blob/05cab639785cbe9a88a11610f9b33bf21cf33f2a/CLAUDE.md
repo: emacs-os/embr.el
kind: claude-md
stars: 68
last_pushed: 2026-05-17T00:49:59Z
license: gpl-3.0
score: 9
domains: [cli-tools, systems-programming, emacs-lisp]
tags: [architecture-heavy, protocol-focused, language-standards]
curated: 2026-06-15
curated_by: config-scout
---

# emacs-os/embr.el — claude-md

**Why it's worth keeping:** It explicitly defines communication protocols, buffer-local state management to prevent side effects, and rigorous coding standards that are highly transferable for complex systems.

**Summary:** Provides deep architectural insights into a client-server system involving Emacs and Python via JSON protocols and frame rendering pipelines.

**Source credibility:** Niche specialized tool with healthy engagement and recent maintenance history.

**Recency:** Current; specifically references modern Emacs 30.1+ features and up-to-date development workflows.

**Source:** [emacs-os/embr.el/CLAUDE.md](https://github.com/emacs-os/embr.el/blob/05cab639785cbe9a88a11610f9b33bf21cf33f2a/CLAUDE.md) · 68★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**embr.el** is an Emacs browser that uses headless Chromium (via CloakBrowser) as its rendering engine. Emacs acts as the display server, while a Python daemon handles browser automation.

## Architecture

Client-server over JSON lines on stdin/stdout:

```
Emacs (embr.el) ←→ JSON over stdin/stdout ←→ Python daemon (embr.py)
  UI / keybindings                            Playwright/CloakBrowser browser control
  Frame display                               CDP screencast or screenshot capture
  Canvas or JPEG rendering                    JPEG frames → file or Unix socket
```

**embr.el** (~2200 lines): Emacs Lisp major mode. Process management, async JSON protocol, two render backends (default + canvas), two frame sources (screencast + screenshot), link hints, tabs, bookmarks, zoom, mute, reader mode, page info, incognito mode.

**embr.py** (~1350 lines): asyncio daemon using CloakBrowser (Playwright API). Browser commands, CDP screencast, screenshot capture loop, canvas frame socket, domain-level ad blocking, extension loading (uBlock Origin, Dark
```

</details>
