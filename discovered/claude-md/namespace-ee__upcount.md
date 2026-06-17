---
name: namespace-ee__upcount
source: https://github.com/namespace-ee/upcount/blob/7b5865950159d12d0c209801f110d7bb7df4aa44/CLAUDE.md
repo: namespace-ee/upcount
kind: claude-md
stars: 387
last_pushed: 2026-05-18T21:18:07Z
license: gpl-3.0
score: 8
domains: [web-frontend, desktop-apps, tauri-rust]
tags: [react, tauri, sqlite, state-management, conventional-commits]
curated: 2026-06-15
curated_by: config-scout
---

# namespace-ee/upcount — claude-md

**Why it's worth keeping:** It details specific state management patterns (Jotai atom patterns) and database interaction methods, plus includes useful git etiquette to prevent AI-generated attribution noise.

**Summary:** Provides comprehensive technical context for a Tauri/React application, focusing on architectural patterns and development workflows.

**Source credibility:** High; the repository has significant stars and recent activity.

**Recency:** Very current; utilizes modern versions of Tauri (2.x) and React Router (7).

**Source:** [namespace-ee/upcount/CLAUDE.md](https://github.com/namespace-ee/upcount/blob/7b5865950159d12d0c209801f110d7bb7df4aa44/CLAUDE.md) · 387★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview
Upcount is a cross-platform invoicing application built with Tauri, React, and SQLite. The app is designed to be offline-first for privacy and supports multiple languages via LinguiJS.

## Architecture
- **Frontend**: React 18 with TypeScript and Vite
- **UI Framework**: Ant Design components
- **State Management**: Jotai atoms for reactive state
- **Backend**: Tauri (Rust) with SQLite database via tauri-plugin-sql
- **Styling**: SCSS with Ant Design theming
- **Internationalization**: LinguiJS with .po files in src/locales/
- **PDF Generation**: @react-pdf/renderer for invoice PDFs

## Key Technologies
- Tauri 2.x for desktop app framework
- React Router 7 for navigation
- Jotai for state management with atoms in src/atoms.tsx
- LinguiJS for i18n with macros for translations
- SQLite with migrations in src-tauri/migrations/

## Development Commands
```bash
# Start development server (runs both Tauri and Vite)
pnpm dev

# Build for production
pnpm tauri build

# Lint TypeScript/React code
pnpm lint

# Extract translation strings
pnpm extract
```
```

</details>
