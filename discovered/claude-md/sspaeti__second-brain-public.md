---
name: sspaeti__second-brain-public
source: https://github.com/sspaeti/second-brain-public/blob/2018da3b406fbcdddfd8c037b87c95231dd677b9/CLAUDE.md
repo: sspaeti/second-brain-public
kind: claude-md
stars: 110
last_pushed: 2026-06-11T19:23:37Z
license: mit
score: 7
domains: [static-site-generator, content-pipeline, devops]
tags: [hugo, obsidian, workflow, automation]
curated: 2026-06-15
curated_by: config-scout
---

# sspaeti/second-brain-public — claude-md

**Why it's worth keeping:** It clearly maps the command hierarchy via makefiles and explicitly distinguishes between legacy (Python) and current (Rust) processing logic to prevent tool confusion.

**Summary:** Defines a custom content pipeline that transforms Obsidian notes into a Hugo static site using Rust and Python utilities.

**Source credibility:** The repository is well-maintained with specific, idiosyncratic automation workflows.

**Recency:** Current; explicitly mentions Claude Code and modern development practices.

**Source:** [sspaeti/second-brain-public/CLAUDE.md](https://github.com/sspaeti/second-brain-public/blob/2018da3b406fbcdddfd8c037b87c95231dd677b9/CLAUDE.md) · 110★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a public second brain website built with Hugo and the Quartz theme (v3). It automatically publishes Obsidian notes tagged with `#publish` from a private vault to a public website hosted at ssp.sh/brain.

## Architecture

- **Hugo Static Site**: Uses Hugo with Quartz theme for generating the public website
- **Content Processing**: Two utility systems process Obsidian notes:
  - Python scripts (`utils/find-publish-notes.py`) - legacy approach
  - Rust utility (`utils/obsidian-quartz/`) - current preferred approach
- **Link Generation**: Uses `hugo-obsidian` (forked version) to generate backlinks and graph connections
- **Deployment**: Static files generated to `public/` and uploaded via rsync

## Core Commands

### Development and Building
```bash
# Start development server (full build + serve)
make serve

# Run Hugo development server only
make run

# Generate static site without serving
make hugo-generate

# Full deployment (build + upload)
make deploy
```

### Content Processing
```bash
# Process notes using Rust utility (preferred)
```

</details>
