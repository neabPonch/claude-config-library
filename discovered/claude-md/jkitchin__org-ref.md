---
name: jkitchin__org-ref
source: https://github.com/jkitchin/org-ref/blob/dc2481d430906fe2552f9318f4405242e6d37396/CLAUDE.md
repo: jkitchin/org-ref
kind: claude-md
stars: 1427
last_pushed: 2025-12-06T14:22:16Z
license: gpl-3.0
score: 9
domains: [editor-extensions, cli-tools]
tags: [emacs-lisp, modular-architecture, performance-optimization]
curated: 2026-06-15
curated_by: config-scout
---

# jkitchin/org-ref — claude-md

**Why it's worth keeping:** The inclusion of 'Common Pitfalls' and deep-dives into performance-critical subsystems (like multi-file label scanning) prevents the AI from introducing architectural or performance regressions.

**Summary:** Maps a complex, modular Emacs Lisp architecture including specific logic for link activation and caching strategies. Provides comprehensive developer workflows for testing, compilation, and environment configuration.

**Source credibility:** High; it is a highly-starred, well-maintained Emacs package with clear documentation structure.

**Recency:** Current; includes modern considerations like native compilation and CI/CD workflows.

**Source:** [jkitchin/org-ref/CLAUDE.md](https://github.com/jkitchin/org-ref/blob/dc2481d430906fe2552f9318f4405242e6d37396/CLAUDE.md) · 1427★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**org-ref** is an Emacs package that provides citations, cross-references, indexes, glossaries, and bibtex utilities for org-mode. It makes academic writing in org-mode convenient by providing hyper-functional links that are clickable, exportable to LaTeX/PDF, and work with completion systems like ivy and helm.

The package is available on MELPA and has ~35 Emacs Lisp modules covering different aspects of functionality.

## Core Architecture

### Module Structure

org-ref follows a modular architecture with clear separation of concerns:

- **org-ref-core.el**: Central hub that requires and orchestrates all major modules. Entry point for most functionality.

- **Link Types** (each provides specific org-mode link functionality):
  - `org-ref-citation-links.el`: Citation links (cite, citeauthor, etc.)
  - `org-ref-ref-links.el`: Cross-reference links (ref, eqref, pageref, etc.)
  - `org-ref-label-link.el`: Label links for marking reference targets
  - `org-ref-bibliography-links.el`: Bibliography and bibliographystyle links
  - `org-ref-misc-links.e
```

</details>
