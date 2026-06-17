---
name: plamere__OrganizeYourMusic
source: https://github.com/plamere/OrganizeYourMusic/blob/c2a1e3b7304429a77fd3678f8c755da81c443b74/CLAUDE.md
repo: plamere/OrganizeYourMusic
kind: claude-md
stars: 270
last_pushed: 2026-02-28T14:51:51Z
license: unknown
score: 8
domains: [web-frontend, api-integration]
tags: [monolith, no-build, architecture-map]
curated: 2026-06-15
curated_by: config-scout
---

# plamere/OrganizeYourMusic — claude-md

**Why it's worth keeping:** It maps out high-level logic sections within a large single file (index.html) and details specific environment-switching requirements for local development.

**Summary:** Provides essential architectural context for a no-build, monolithic single-page application.

**Source credibility:** The 270 stars suggest this is a functional, real-world utility.

**Recency:** Current; the instructions are highly relevant to modern LLM-assisted development of legacy or minimal architectures.

**Source:** [plamere/OrganizeYourMusic/CLAUDE.md](https://github.com/plamere/OrganizeYourMusic/blob/c2a1e3b7304429a77fd3678f8c755da81c443b74/CLAUDE.md) · 270★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Organize Your Music is a client-side Spotify web app that lets users organize their saved music, playlists, and followed playlists by attributes like genre, mood, decade, popularity, and audio features (energy, danceability, etc.). Users can browse organized "bins," preview tracks, and save selections as new Spotify playlists.

## Architecture

This is a **no-build, single-page web app**. All application logic lives as inline JavaScript in `web/index.html` (~2400 lines). There is no build system, bundler, or package manager.

**Key files:**
- `web/index.html` — The entire app: HTML, CSS overrides, and all JS logic inline
- `web/config.js` — Spotify OAuth client ID and redirect URIs
- `web/styles2.css` — Custom styles (on top of Spotify Bootstrap theme)
- `web/lib/` — Vendored JS libraries (jQuery, Underscore, Moment, RSVP, Typeahead)
- `web/deploy` — Shell script to deploy via `s3cmd sync` to S3

**External dependencies (loaded via CDN):**
- Spotify Bootstrap CSS/JS, Font Awesome, Google Charts, Plotly, x-editable

**Spotify API integration:**
-
```

</details>
