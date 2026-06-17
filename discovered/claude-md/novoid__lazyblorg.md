---
name: novoid__lazyblorg
source: https://github.com/novoid/lazyblorg/blob/3992d1049d9e7773fb15fe24625b493a64678ea2/CLAUDE.md
repo: novoid/lazyblorg
kind: claude-md
stars: 436
last_pushed: 2026-04-14T02:57:22Z
license: gpl-3.0
score: 8
domains: [cli-tools, static-site-generators, python]
tags: [org-mode, architecture-docs, business-rules]
curated: 2026-06-15
curated_by: config-scout
---

# novoid/lazyblorg — claude-md

**Why it's worth keeping:** The 'Blog entry requirements' section is an excellent pattern for documenting invisible business logic that would otherwise cause errors, and the architectural data flow breakdown prevents hallucinations regarding component interactions.

**Summary:** Defines specific domain rules for valid blog entries and provides comprehensive command patterns for testing/running via uv. It maps out a clear data flow from Org files through the parser to HTML.

**Source credibility:** High; 436 stars indicates a widely used tool with recent maintenance.

**Recency:** Very current; uses modern tooling like `uv` and Python 3.13.

**Source:** [novoid/lazyblorg/CLAUDE.md](https://github.com/novoid/lazyblorg/blob/3992d1049d9e7773fb15fe24625b493a64678ea2/CLAUDE.md) · 436★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What is lazyblorg

A static blog generator that converts Org-mode files into HTML5. Blog entries are scattered throughout regular Org-mode files (no dedicated blog file needed). Uses pickle-based metadata to track changes and only regenerate what's needed.

Any user-visible text should not be included into the Python files. Instead, templates should be used for any text and `config.org` for any site-specific configuration. This way, most translation should happen in the template files and not within the Python code.

On any change, also update the Org-mode time-stamp in lazyblorg.py: `PROG_VERSION = "Time-stamp: <2020-10-03 19:51:01 vk>"`: Make sure that the date matches the current date and the time stamp matches the current time.

If the Atom feeds are changed, ask back the user if this change is OK since the feeds are used by the public already.

## Build & Run Commands

```bash
# Run tests (unit + integration)
uv --project . run pytest

# Run end-to-end tests
./start_end-to-end-test.sh

# Run all tests
./start_all_tests.sh

# Run a single test file
uv --projec
```

</details>
