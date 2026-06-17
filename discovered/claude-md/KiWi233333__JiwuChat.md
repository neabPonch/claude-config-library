---
name: KiWi233333__JiwuChat
source: https://github.com/KiWi233333/JiwuChat/blob/63458b9c34a29ef17a6e61873f63c587d82bfc6c/CLAUDE.md
repo: KiWi233333/JiwuChat
kind: claude-md
stars: 718
last_pushed: 2026-05-20T18:47:03Z
license: agpl-3.0
score: 9
domains: [web-frontend, desktop-app, cross-platform]
tags: [nuxt, tauri, vue3, unocss]
curated: 2026-06-15
curated_by: config-scout
---

# KiWi233333/JiwuChat — claude-md

**Why it's worth keeping:** It contains highly specific 'known pitfalls' (like the el-tooltip bug) and unique styling rules for UnoCSS usage that prevent common developer errors. The explicit instruction on how component names are derived from directory paths is excellent context for an AI.

**Summary:** A comprehensive technical guide for a Nuxt/Tauri cross-platform application that includes precise environment versions, command mappings, and architectural patterns.

**Source credibility:** Strong; a popular open-source project with high star count and recent maintenance.

**Recency:** 

**Source:** [KiWi233333/JiwuChat/CLAUDE.md](https://github.com/KiWi233333/JiwuChat/blob/63458b9c34a29ef17a6e61873f63c587d82bfc6c/CLAUDE.md) · 718★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

本文件为在仓库中编写、修改代码时提供统一规范与上下文，供 Claude Code 及协作者遵循。全程中文进行回答和编码相关

## Project Overview

JiwuChat 是基于 Tauri 2.9+ 与 Nuxt.js 4.0 的跨平台聊天应用，支持桌面、Web、移动端；轻量（约 10MB），集成 AI、WebRTC 与多平台 OAuth。

## Technology Stack

- **Frontend**: Nuxt.js 4.2 + Vue 3 + TypeScript 5.9.3 + Element Plus 2.13.1 + UnoCSS + Pinia 3.0.4
- **Desktop**: Tauri 2.9+ (Rust)
- **Rich Text**: TipTap（markdown、@ 提及、表格、任务列表）
- **Markdown**: md-editor-v3 5.8.4
- **Package Manager**: pnpm 10.13.1（必须）
- **Node.js**: 22.20.0（Volta 管理）
- **Build**: Vite + Rolldown（rolldown-vite@7.2.11）

## Essential Development Commands

### Development

```bash
pnpm run dev:nuxt          # Web 开发（最常用）
pnpm run dev:vscode:nuxt   # Web + VS Code 调试
pnpm run dev:tauri         # 桌面开发（或 dev:desktop）
pnpm run dev:android       # Android
pnpm run dev:ios           # iOS（仅 macOS）
pnpm run prod:nuxt         # 生产环境本地验证
pnpm run prod:nuxt:local
```

### Building

```bash
pnpm run build       # 全量构建（Web + 桌面）
pnpm run build:nuxt  # 仅 Web
pnpm run build:tauri # 仅桌面
```

### Code Quality

```bash
pnpm run lint:fix              # 提交前执行
cd src-tauri && cargo check    # Rust 类型检查
```

### Mobile

```bash
pnpm run android-init
pnpm run ios-init   # 仅 ma
```

</details>
