---
name: IIRoan__manganess
source: https://github.com/IIRoan/manganess/blob/9d9c6436cecac62666a2660d3c3ea0e15cf962d6/claude.md
repo: IIRoan/manganess
kind: claude-md
stars: 6
last_pushed: 2026-06-12T19:11:14Z
license: 0bsd
score: 9
domains: [mobile-development, react-native, frontend]
tags: [expo, typescript, architecture, patterns]
curated: 2026-06-15
curated_by: config-scout
---

# IIRoan/manganess — claude-md

**Why it's worth keeping:** The explicit 'Component Architecture Pattern' provides a perfect boilerplate that enforces memoization, theme integration, and specific import ordering, preventing AI-generated code drift.

**Summary:** A highly detailed guide establishing strict architectural patterns, component blueprints, and styling conventions for a React Native Expo application.

**Source credibility:** Reliable; reflects an active, well-structured open-source project with modern dependencies.

**Recency:** Very recent; uses Expo SDK 54 and React 19, making it highly relevant for modern development environments.

**Source:** [IIRoan/manganess/claude.md](https://github.com/IIRoan/manganess/blob/9d9c6436cecac62666a2660d3c3ea0e15cf962d6/claude.md) · 6★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# MangaNess AI Agent Development Guide

## Project Overview

MangaNess is a React Native manga reading application built with Expo SDK 54, featuring a clean, ad-free reading experience with AniList integration, bookmark management, and comprehensive theming support.

### Core Technologies

- **React Native 0.81.4** with **React 19.1.0**
- **Expo SDK 54** with Expo Router for file-based navigation
- **TypeScript** with strict configuration
- **Bun** as package manager and runtime
- **AsyncStorage** for local data persistence
- **Axios** for HTTP requests

## Architecture Overview

### File-Based Routing Structure

```
app/
├── _layout.tsx                 # Root layout with providers
├── (tabs)/                     # Tab-based navigation
│   ├── _layout.tsx            # Tab layout with swipe gestures
│   ├── index.tsx              # Home screen
│   ├── mangasearch.tsx        # Search functionality
│   ├── bookmarks.tsx          # Bookmark management
│   ├── settings.tsx           # App settings
│   └── manga/[id]/            # Dynamic manga routes
│       ├── index.tsx          # Manga details page
│       └── chapter/[chapterNumber].tsx  # Chapter reader
```

### Core Directory Stru
```

</details>
