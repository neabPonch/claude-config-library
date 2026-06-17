---
name: plamere__playlistminer
source: https://github.com/plamere/playlistminer/blob/4b828928f3c20dc0afaa4780793d293bd429a1c4/CLAUDE.md
repo: plamere/playlistminer
kind: claude-md
stars: 157
last_pushed: 2026-03-18T10:47:03Z
license: unknown
score: 9
domains: [web-frontend, api-integration]
tags: [spotify-api, vanilla-js, technical-documentation]
curated: 2026-06-16
curated_by: config-scout
---

# plamere/playlistminer — claude-md

**Why it's worth keeping:** Includes critical domain-specific knowledge like Spotify's pagination/rate-limiting quirks and local development IP requirements. The 'Key Flow' section provides an excellent mental model for LLM reasoning.

**Summary:** Provides a high-fidelity technical manual for a single-page application including specific API behavior and deployment workflows. It maps out the entire data lifecycle from auth to track aggregation.

**Source credibility:** A well-documented repository with a significant star count for its niche.

**Recency:** The documentation strategy is highly effective for modern agentic workflows regardless of the legacy tech stack.

**Source:** [plamere/playlistminer/CLAUDE.md](https://github.com/plamere/playlistminer/blob/4b828928f3c20dc0afaa4780793d293bd429a1c4/CLAUDE.md) · 157★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

The Playlist Miner is a client-side web app that finds the most popular tracks across Spotify playlists matching a keyword search. Users log in with Spotify, enter search terms (e.g. "workout"), and the app aggregates tracks from up to 1000 matching playlists to surface the top 100 most frequently occurring songs, which can be saved as a new Spotify playlist.

## Architecture

**Single-page app** — all application logic lives inline in `index.html` as vanilla JavaScript (jQuery + Underscore.js). There is no build step, bundler, or framework.

### Key flow:
1. **Auth**: Spotify OAuth Authorization Code + PKCE flow (`authorizeUser()` / `exchangeCodeForToken()`). Refresh token cached in `localStorage` for session persistence across page loads.
2. **Playlist search**: `findMatchingPlaylists()` — searches Spotify API for playlists matching keywords, paging sequentially via Spotify's `next` URL. Includes 429 retry with `Retry-After` backoff.
3. **Track aggregation**: `fetchAllTracksFromPlaylist()` — fetches tracks from each playlist (max 6 simultaneous
```

</details>
