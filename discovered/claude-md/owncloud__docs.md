---
name: owncloud__docs
source: https://github.com/owncloud/docs/blob/6ceaf02dba2e3d2ae48804f9d3f90e9886052ea7/CLAUDE.md
repo: owncloud/docs
kind: claude-md
stars: 56
last_pushed: 2026-06-15T15:15:01Z
license: agpl-3.0
score: 9
domains: [documentation, static-site-generators]
tags: [asciidoc, antora, docs-as-code]
curated: 2026-06-16
curated_by: config-scout
---

# owncloud/docs — claude-md

**Why it's worth keeping:** It provides granular rules for internal linking, image pathing, and SEO preservation (page aliases) that prevent broken builds or broken links during content updates.

**Summary:** Defines build workflows and highly specific AsciiDoc syntax requirements for an Antora-based documentation repository.

**Source credibility:** High; comes from a mature, well-maintained open-source project (ownCloud).

**Recency:** Current; includes modern toolchain commands and specific versioning context.

**Source:** [owncloud/docs/CLAUDE.md](https://github.com/owncloud/docs/blob/6ceaf02dba2e3d2ae48804f9d3f90e9886052ea7/CLAUDE.md) · 56★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

This is the ownCloud Server documentation repository. It uses **Antora** (static site generator) with **AsciiDoc** (`.adoc`) format. The current component is `server` version `10.4`.

## Build Commands

```bash
# Install dependencies
yarn install

# Build HTML documentation
yarn antora

# Validate internal cross-references (xrefs)
yarn validate

# Lint prose in AsciiDoc files
yarn prose

# Check for broken links (requires built site)
yarn linkcheck

# Serve the built docs locally at http://localhost:8080
yarn serve
```

## Content Structure

Antora organizes content into **modules**, each with a fixed directory layout:

```
modules/<module_name>/
  pages/         # AsciiDoc source files (.adoc)
  assets/images/ # Images
  examples/      # Code examples and included files
  nav.adoc       # Module navigation
```

The four modules are: `ROOT`, `admin_manual`, `user_manual`, `developer_manual`.

## AsciiDoc Conventions

**Internal links** use `xref:` (never Markdown-style links):
```asciidoc
xref:module_name:path/file.adoc#anchor[Link Text]
# module_name: i
```

</details>
