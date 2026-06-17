---
name: XuYouo__MeowNocode
source: https://github.com/XuYouo/MeowNocode/blob/b5275e3a624a7a682c3123112606581e115fd020/CLAUDE.md
repo: XuYouo/MeowNocode
kind: claude-md
stars: 453
last_pushed: 2026-01-24T07:33:15Z
license: mit
score: 9
domains: [web-frontend, fullstack, backend-api]
tags: [react, cloudflare-d1, sqlite, vite]
curated: 2026-06-15
curated_by: config-scout
---

# XuYouo/MeowNocode — claude-md

**Why it's worth keeping:** The explicit distinction between deployment models and the detailed breakdown of API endpoints and DB schema prevent hallucinated backend logic.

**Summary:** A comprehensive full-stack guide covering multiple deployment targets (Cloudflare vs. Self-hosted) and database schemas.

**Source credibility:** High; well-structured open-source project with significant popularity (453 stars).

**Recency:** Modern; uses current tech like React 18, Vite, and TanStack Query.

**Source:** [XuYouo/MeowNocode/CLAUDE.md](https://github.com/XuYouo/MeowNocode/blob/b5275e3a624a7a682c3123112606581e115fd020/CLAUDE.md) · 453★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

MeowNocode is a lightweight, privacy-focused note-taking application with canvas mode, heatmap statistics, AI chat, and cloud sync capabilities. It supports multiple deployment models and storage backends.

**Key Features:**
- Canvas mode for spatial note organization
- GitHub-style heatmap for tracking productivity
- Markdown support with syntax highlighting
- Tag management and backlink system
- Audio clip attachments to notes
- Music player with playlist support
- AI-powered chat integration
- Cloud sync with Cloudflare D1 or Supabase
- Self-hosted SQLite option

## Architecture

This is a **full-stack application** with three deployment models:

### 1. Frontend (React + Vite)
- **Framework:** React 18 with Vite build tool
- **UI Library:** Radix UI components with Tailwind CSS
- **State Management:** React Context (SettingsContext, ThemeContext, MusicContext, PasswordAuthContext)
- **Routing:** React Router DOM
- **Data Fetching:** TanStack React Query
- **Styling:** Tailwind CSS with `cn()` utility from `src/lib/utils.js`

### 2. Cloudflare
```

</details>
