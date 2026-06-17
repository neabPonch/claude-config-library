---
name: vijaythecoder__clueless
source: https://github.com/vijaythecoder/clueless/blob/28eaae90c3d515e9a3eb344444dc4574c0a98e65/CLAUDE.md
repo: vijaythecoder/clueless
kind: claude-md
stars: 582
last_pushed: 2026-01-09T02:12:28Z
license: other
score: 9
domains: [fullstack-web, desktop-app, ai-integration]
tags: [laravel, vue, nativephp, realtime-api]
curated: 2026-06-15
curated_by: config-scout
---

# vijaythecoder/clueless — claude-md

**Why it's worth keeping:** Includes crucial specific instructions for dual-database migrations (NativePHP) and explains the custom WebSocket architecture to prevent incorrect refactoring attempts.

**Summary:** A highly detailed guide that covers tech stack, architecture patterns, and critical runtime nuances. It excels at providing 'gotcha' instructions for non-standard development workflows.

**Source credibility:** Highly credible; part of a popular open-source project with significant star count.

**Recency:** Extremely current, referencing modern versions like Laravel 12 and Tailwind 4.

**Source:** [vijaythecoder/clueless/CLAUDE.md](https://github.com/vijaythecoder/clueless/blob/28eaae90c3d515e9a3eb344444dc4574c0a98e65/CLAUDE.md) · 582★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Clueless is an AI-powered meeting assistant that provides real-time transcription, intelligent analysis, and action item extraction from conversations. It's built as a single-user desktop application using Electron/NativePHP with OpenAI's Realtime API for voice conversations.

## Tech Stack

- **Backend**: Laravel 12.0 (PHP 8.2+)
- **Frontend**: Vue 3.5.13 with TypeScript and Inertia.js
- **CSS**: Tailwind CSS 4.1.1
- **Build**: Vite 6
- **Desktop**: NativePHP/Electron
- **Testing**: Pest PHP
- **Database**: SQLite (dual database setup)
- **Real-time**: OpenAI Realtime API, WebSockets
- **AI Integration**: OpenAI Realtime API only

## Development Commands

### Running the Application

```bash
# Full development environment (Laravel + Vite + Queue + Logs)
composer dev

# Development with Server-Side Rendering
composer dev:ssr

# Desktop application mode (NativePHP)
composer native:dev

# Frontend only (Vite dev server)
npm run dev
```

### Build Commands

```bash
# Build frontend for production
npm run build

# Build with SSR support
npm run build
```

</details>
