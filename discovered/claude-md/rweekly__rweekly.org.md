---
name: rweekly__rweekly.org
source: https://github.com/rweekly/rweekly.org/blob/cfb9b8c75b15d5eba42281de71821fef839ea7d0/CLAUDE.md
repo: rweekly/rweekly.org
kind: claude-md
stars: 815
last_pushed: 2026-06-14T00:24:37Z
license: unknown
score: 9
domains: [static-site, automation, data-processing, r-programming]
tags: [jekyll, r-language, nix, content-pipeline]
curated: 2026-06-15
curated_by: config-scout
---

# rweekly/rweekly.org — claude-md

**Why it's worth keeping:** Includes highly practical tool fallbacks (Jina/Defuddle) for web fetching and provides exact shell commands to execute repository-specific automation.

**Summary:** Provides comprehensive documentation for site architecture, internal R automation scripts, and the specific content structure required for a weekly newsletter.

**Source credibility:** High; the project is active and well-starred with clear, specialized utility scripts.

**Recency:** Very current; integrates modern dev-ops practices like Nix and specific guidance for Claude Code's capabilities.

**Source:** [rweekly/rweekly.org/CLAUDE.md](https://github.com/rweekly/rweekly.org/blob/cfb9b8c75b15d5eba42281de71821fef839ea7d0/CLAUDE.md) · 815★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Repository Is

This is the source for [rweekly.org](https://rweekly.org), a weekly community-curated newsletter about the R programming language. It is a Jekyll-based static site hosted on GitHub Pages (`gh-pages` branch is the main branch).

## Site Architecture

- **Jekyll site**: `_config.yml` configures the site, `_layouts/` holds HTML templates, `_includes/` holds partials and static assets (CSS/JS vendored inline).
- **Published posts**: `_posts/` — one Markdown file per weekly issue, named `YYYY-MM-DD-<issue>.md`.
- **Current draft**: `draft.md` — the live working draft for the next issue. Contributors submit PRs adding links here.
- **RSS feed list**: `rss_feeds.csv` — CSV with columns `URL`, `ENABLE`, `TWITTER`. New blog feeds are added here (set `ENABLE=1`).
- **R scripts**: `scripts/` — automation scripts for content collection and processing.

## Draft Post Format

Links in `draft.md` (and posts) use this format:
```
+ [Title](URL) - optional description

![Optional image alt text](image-URL)
```

Sections in the draft: Highlight, Insights, R
```

</details>
