---
name: chrisbirster__flashcards
source: https://github.com/chrisbirster/flashcards/blob/f686c684e1e740480b8db931989ef98ce298bec6/claude.md
repo: chrisbirster/flashcards
kind: claude-md
stars: 1
last_pushed: 2026-05-26T01:03:25Z
license: other
score: 9
domains: [mobile-app, fullstack, react-native]
tags: [expo, typescript, roadmap, pattern-driven]
curated: 2026-06-15
curated_by: config-scout
---

# chrisbirster/flashcards — claude-md

**Why it's worth keeping:** Features an excellent 'Milestone Progress Tracking' system for managing agent state and provides highly specific patterns like import aliases and React Compiler memoization rules.

**Summary:** A highly detailed full-stack guide covering architectural rules, specific code patterns, and a living task roadmap.

**Source credibility:** Low star count suggests a personal project, but the technical density is high.

**Recency:** Extremely current, referencing modern Expo versions and the new React Compiler.

**Source:** [chrisbirster/flashcards/claude.md](https://github.com/chrisbirster/flashcards/blob/f686c684e1e740480b8db931989ef98ce298bec6/claude.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Microdote — Project Context

## Project Overview

**Microdote** is a web-based reimplementation of Anki's spaced repetition flashcard system. The goal is to achieve feature parity with Anki while providing a modern, cross-platform experience through a React Native mobile app with a Go backend.

The complete feature roadmap and task breakdown is maintained in `microdote_anki_tasks.md`, which maps all Anki Manual features into 8 major milestones (M0-M8) with detailed acceptance criteria and dependencies.

## Tech Stack

### Frontend (Mobile App)
- **React Native 0.81** with **Expo 54**
- **TypeScript** for type safety
- **React Navigation** for routing and navigation
- **TanStack Query (React Query)** for data fetching and cache management

### Backend
- **Go** (see `go.mod` for version and dependencies)
- RESTful API serving the React Native frontend

### Storage
- Planning to use IndexedDB/SQLite-in-browser or remote database (see Task 0002 in task plan)

## Project Structure

```
/flashcards
├── main.go                      # Go backend server
├── go.mod, go.sum              # Go dependencies
├── web/                        # React Native frontend
├── microdote_anki_tasks.md
```

</details>
