---
name: Awful-Security__awful_security_news
source: https://github.com/Awful-Security/awful_security_news/blob/6d2dd5b259870e65d0f0bc53668f70213abf5325/CLAUDE.md
repo: Awful-Security/awful_security_news
kind: claude-md
stars: 8
last_pushed: 2025-12-06T10:43:06Z
license: mit
score: 9
domains: [automation, content-pipeline, data-engineering]
tags: [ascii-diagrams, build-orchestration, external-dependencies, justfile]
curated: 2026-06-16
curated_by: config-scout
---

# Awful-Security/awful_security_news — claude-md

**Why it's worth keeping:** The ASCII architecture diagram provides essential system-level visibility into data movement, and the 'External Binaries' section solves the common issue of missing non-repo dependencies.

**Summary:** A high-context guide for a complex automated media pipeline that maps data flows and build orchestration.

**Source credibility:** Solid; specialized niche project with recent maintenance (last 6 months) and clear authorship.

**Recency:** Highly current; uses modern toolchains like `just` and includes 2025 context/data.

**Source:** [Awful-Security/awful_security_news/CLAUDE.md](https://github.com/Awful-Security/awful_security_news/blob/6d2dd5b259870e65d0f0bc53668f70213abf5325/CLAUDE.md) · 8★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md - Awful Security News Repository Guide

## Project Overview

**Awful Security News** is an automated daily news aggregation and narrative analysis platform. It fetches security/technology news from multiple sources, summarizes articles using an LLM (Qwen 3 4B), generates D3.js visualizations analyzing media narratives, and publishes everything through an mdBook-based static site with Elasticsearch search.

- **Website:** https://news.awfulsec.com
- **Repository:** github.com/graves/awful_security_news
- **Author:** Thomas Graves

## Quick Reference Commands

```bash
# Build and deploy
just run-edition          # Full build pipeline (default)
just build-only           # Build without Elasticsearch indexing
just force-vibes          # Generate viz data (ignores morning-only restriction)
just update-viz-index     # Regenerate viz/index.json from existing data

# Docker services
just up                   # Start Elasticsearch
just down                 # Stop services
just restart              # Restart services
just status               # Show container status
just logs                 # View all logs
just es-status            # Check Elasticsearch health

# Utilities
just
```

</details>
