---
name: emdmed__terminal-notes
source: https://github.com/emdmed/terminal-notes/blob/a6cc7e4dda9d058c04b1825a1107950e245c2412/claude.md
repo: emdmed/terminal-notes
kind: claude-md
stars: 0
last_pushed: 2025-11-18T22:13:10Z
license: unknown
score: 9
domains: [cli-tools, web-frontend, nodejs]
tags: [architecture, tui, vim-keys]
curated: 2026-06-14
curated_by: config-scout
---

# emdmed/terminal-notes — claude-md

**Why it's worth keeping:** The 'Development Decisions' section is a masterclass in providing intent-based context; the 'Common Patterns' section provides clear implementation blueprints for new components.

**Summary:** This document provides a deep architectural mental model including state management logic, data schemas, and specific keyboard interaction patterns. It excels at explaining the 'why' behind design trade-offs rather than just describing what the code does.

**Source credibility:** Zero stars, but the extreme documentation density suggests a highly disciplined developer.

**Recency:** 7 months old; remains highly relevant for modern React/Node development and Claude Code usage.

**Source:** [emdmed/terminal-notes/claude.md](https://github.com/emdmed/terminal-notes/blob/a6cc7e4dda9d058c04b1825a1107950e245c2412/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Development Notes

This document contains Claude-specific context about the terminal-notes codebase, development decisions, and architectural patterns.

## Project Overview

A vim-style terminal note-taking application built with React and Ink. The app uses a TUI (Terminal User Interface) for managing notes with vim keybindings and a priority system.

## Architecture

### Component Structure

The application follows a simple React component architecture with three main views:

- **NoteListView** - Main list view showing all notes with navigation and sorting
- **NoteEditor** - Dual-mode component (view/edit) for displaying and editing notes
- **DeleteConfirmation** - Confirmation dialog for note deletion

### State Management

All state is managed in `app.js` using React hooks:
- `view` - Current view state ('list', 'edit', 'delete')
- `notes` - Array of all notes loaded from storage
- `selectedNoteId` - Currently selected note ID
- `editorMode` - Whether NoteEditor opens in 'view' or 'edit' mode
- `sortMode` - Current sort configuration ('priority-asc', 'priority-desc', 'date-asc', 'date-desc')

### Data Storage

Notes are persisted to `~/.terminal_notes.json` as a JSON ar
```

</details>
