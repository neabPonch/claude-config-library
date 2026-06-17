---
name: xinggaoya__sing-box-windows
source: https://github.com/xinggaoya/sing-box-windows/blob/14d30591ffcdeac49f1c92350702f98a20133666/CLAUDE.md
repo: xinggaoya/sing-box-windows
kind: claude-md
stars: 765
last_pushed: 2026-05-27T08:03:45Z
license: mit
score: 9
domains: [desktop-app, fullstack, rust, web-frontend]
tags: [tauri, rust, vue, architecture-driven]
curated: 2026-06-15
curated_by: config-scout
---

# xinggaoya/sing-box-windows — claude-md

**Why it's worth keeping:** The 'Development Workflow' section offers explicit step-by-step instructions for adding features, while the 'Core Architecture' explains critical state management and communication patterns that an LLM would likely misinterpret without guidance.

**Summary:** Provides a highly structured blueprint for a complex Tauri/Rust/Vue application by defining architectural patterns rather than just file lists.

**Source credibility:** High; a well-starred (765) active repository with modern tech stacks.

**Recency:** Current; utilizes Tauri 2.0 and up-to-date frontend tooling.

**Source:** [xinggaoya/sing-box-windows/CLAUDE.md](https://github.com/xinggaoya/sing-box-windows/blob/14d30591ffcdeac49f1c92350702f98a20133666/CLAUDE.md) · 765★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 开发指导原则

- 请你全程使用中文进行交流
- 代码过程中在必要的地方要写一些注释
- 如果涉及到编写页面，请你以现代化、简约、美观的风格设计
- 你可以使用任何工具、以及MCP在开发时最好使用MCP熟悉最新文档

## Project Overview

sing-box-windows is a modern cross-platform proxy client for Windows, Linux, and macOS built with Tauri 2.0 + Vue 3, providing complete proxy management, routing rules, subscription management, and system service functionality.

### Tech Stack

- **Frontend**: Vue 3 + TypeScript + Vite + Pinia + Naive UI
- **Backend**: Rust + Tauri 2.0 + tokio
- **Architecture**: MVVM + modular design
- **Persistence**: Tauri Store (replaces localStorage) + SQLite database
- **Build**: Vite (frontend) + cargo-cp-artifact (Rust backend)

## Common Commands

### Development
```bash
# Install dependencies
pnpm install
cd src-tauri && cargo fetch

# Start development server
pnpm tauri dev
```

### Build and Packaging
```bash
# Build production version
pnpm tauri build

# Build MSI installer (Windows)
pnpm tauri build:windows

# Build DEB package (Linux)
pnpm tauri build:linux:deb

# Build AppImage (Linux)
pnpm tauri build:linux:appimage

# Build DMG (macOS)
```

</details>
