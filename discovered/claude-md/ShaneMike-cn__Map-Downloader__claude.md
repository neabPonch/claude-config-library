---
name: ShaneMike-cn__Map-Downloader__claude
source: https://github.com/ShaneMike-cn/Map-Downloader/blob/fb2ba213becea35e36b4defca2b1c1257668daa6/my-tiler-ui/CLAUDE.md
repo: ShaneMike-cn/Map-Downloader
kind: claude-md
stars: 6
last_pushed: 2026-02-12T12:23:43Z
license: apache-2.0
score: 7
domains: [web-frontend, mapping]
tags: [vue-3, vite, leaflet, api-integration]
curated: 2026-06-15
curated_by: config-scout
---

# ShaneMike-cn/Map-Downloader — claude-md

**Why it's worth keeping:** It explicitly maps out the interaction between frontend panels and specific API endpoints, which prevents an agent from hallucinating incorrect network requests.

**Summary:** Provides a clear architectural breakdown of a Vue 3 map tile downloader including UI components and backend endpoints.

**Source credibility:** Low star count but high-quality, human-written documentation style.

**Recency:** Current; reflects modern Vite/Vue 3 development standards.

**Source:** [ShaneMike-cn/Map-Downloader/my-tiler-ui/CLAUDE.md](https://github.com/ShaneMike-cn/Map-Downloader/blob/fb2ba213becea35e36b4defca2b1c1257668daa6/my-tiler-ui/CLAUDE.md) · 6★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Vue 3 application built with Vite that serves as a map tile downloader UI. The application allows users to:
- Select map sources (Google Maps, TianDiTu, ArcGIS, etc.)
- Define geographic regions using Chinese administrative divisions
- Configure zoom levels for tile downloading
- Set up MinIO storage for tile uploads
- Preview downloaded tiles

## Key Technologies

- Vue 3 with Composition API (`<script setup>`)
- Vite build tool
- TypeScript (used in App.vue but no .ts files)
- Leaflet for map preview
- AMap (Gaode Map) API for region selection
- Element Plus UI components
- Axios for HTTP requests

## Project Structure

```
my-tiler-ui/
├── src/
│   ├── main.js          # Entry point
│   └── App.vue          # Main application component
├── public/              # Static assets
├── package.json         # Dependencies and scripts
└── vite.config.js       # Vite configuration
```

## Development Commands

### Install Dependencies
```bash
npm install
```

### Start Development Server
```bash
npm run dev
```
Default URL: http://localhost:5
```

</details>
