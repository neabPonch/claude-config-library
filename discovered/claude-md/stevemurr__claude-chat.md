---
name: stevemurr__claude-chat
source: https://github.com/stevemurr/claude-chat/blob/dfe309c7f752cacbe0ebf8b585e935fad0691fea/claude.md
repo: stevemurr/claude-chat
kind: claude-md
stars: 0
last_pushed: 2026-03-01T17:33:57Z
license: mit
score: 8
domains: [macOS, swift-ui, cli-tools]
tags: [architecture, build-process, subprocess]
curated: 2026-06-17
curated_by: config-scout
---

# stevemurr/claude-chat — claude-md

**Why it's worth keeping:** Provides critical architectural details like JSON streaming logic, specific build dependencies (xcodegen), and vital file paths for persistent data.

**Summary:** A technical guide for a macOS application that interfaces with the Claude Code CLI via subprocesses.

**Source credibility:** Low-star repository but contains high-density, non-generic technical documentation.

**Recency:** Recent; published within the last 4 months.

**Source:** [stevemurr/claude-chat/claude.md](https://github.com/stevemurr/claude-chat/blob/dfe309c7f752cacbe0ebf8b585e935fad0691fea/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# ClaudeChat Development Guide

## Project Overview

ClaudeChat is a native macOS app that provides a floating chat interface for Claude Code CLI. It runs as a menu bar agent with global hotkey support.

## Tech Stack

- **Swift 5.9** / **SwiftUI** - Native macOS app
- **xcodegen** - Xcode project generation from `project.yml`
- **MarkdownUI** - Markdown rendering for chat responses
- **Tiptap** - Rich text editor for notes (via WKWebView)

## Key Architecture

### Chat System
- `ClaudeService` spawns `claude -p` subprocess with `--output-format stream-json`
- Streaming JSON responses are parsed in real-time
- Sessions persist with conversation ID for context continuity

### Notes System
- `NoteService` manages note CRUD with JSON persistence
- `TiptapEditorView` wraps a WebView running Tiptap editor
- Notes stored as markdown with block-based internal representation
- `TitleService` uses Claude to auto-generate note titles

### Command Palette
- `CommandPaletteService` provides fuzzy search across notes and chats
- Keyboard-driven navigation with `Cmd+K` to open

## Building

```bash
# Generate Xcode project
xcodegen generate

# Open in Xcode
open ClaudeChat.xcodeproj

# Build and
```

</details>
