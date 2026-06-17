---
name: mikaelweiss__openchat
source: https://github.com/mikaelweiss/openchat/blob/57762ba0d1c5554952f0f13fc9e080f59caf810b/CLAUDE.md
repo: mikaelweiss/openchat
kind: claude-md
stars: 2
last_pushed: 2026-05-20T23:13:41Z
license: other
score: 9
domains: [desktop-app, web-frontend, rust, cross-platform]
tags: [tauri, react, typescript, sqlite, bun]
curated: 2026-06-15
curated_by: config-scout
---

# mikaelweiss/openchat — claude-md

**Why it's worth keeping:** Includes crucial 'meta-knowledge' like hot-reload behavior to prevent redundant tasks, specific DB schema definitions, and strict changelog maintenance rules.

**Summary:** A highly detailed technical blueprint covering architecture, database schemas, and specific development workflows for a Tauri-based application.

**Source credibility:** High quality personal project with professional documentation standards.

**Recency:** Very current; utilizes modern tech like Bun and Tauri v2.

**Source:** [mikaelweiss/openchat/CLAUDE.md](https://github.com/mikaelweiss/openchat/blob/57762ba0d1c5554952f0f13fc9e080f59caf810b/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Open Chat is a modern desktop AI chat application built with Tauri v2, React, TypeScript, and Tailwind CSS. It's designed as a cross-platform client for communicating with various AI providers (Anthropic Claude, OpenAI, local models via Ollama, etc.).

## Development Commands

### Core Commands
- `bun tauri dev` - Start development server with hot reload
- `bun tauri build` - Build production application
- `bun dev` - Start frontend development server only (without Tauri)
- `bun run build` - Build frontend assets only

### Mobile Development
- `bun tauri ios dev` - iOS simulator development
- `bun tauri android dev` - Android emulator development

### Prerequisites
- Install Rust: `curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh`
- Install Bun: `curl -fsSL https://bun.sh/install | bash`
- Install dependencies: `bun install`

## Architecture

### Data Layer
The app uses a dual-storage approach:
- **SQLite Database** (`src/shared/chatStore.ts`): Manages conversations, messages, and AI provider configurations
- **Key-Value Store** (`s
```

</details>
