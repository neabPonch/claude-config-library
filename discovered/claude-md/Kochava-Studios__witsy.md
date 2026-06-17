---
name: Kochava-Studios__witsy
source: https://github.com/Kochava-Studios/witsy/blob/c81c7de417a6362825bced2e865184d6e3fb73ba/CLAUDE.md
repo: Kochava-Studios/witsy
kind: claude-md
stars: 1981
last_pushed: 2026-04-23T17:32:21Z
license: agpl-3.0
score: 9
domains: [desktop-app, electron, vue-js, typescript]
tags: [architecture, workflow-constraints, ipc, testing-patterns]
curated: 2026-06-16
curated_by: config-scout
---

# Kochava-Studios/witsy — claude-md

**Why it's worth keeping:** The inclusion of 'negative constraints' (e.g., Never run build/E2E) prevents the agent from wasting time on slow tasks, while specific IPC and event bus pattern instructions reduce implementation hallucinations.

**Summary:** A highly structured guide that combines architectural overview with strict operational constraints and specific development patterns.

**Source credibility:** High; a popular open-source project with significant stars and recent maintenance.

**Recency:** Current; tailored for modern tool use by explicitly guiding incremental development and testing flows.

**Source:** [Kochava-Studios/witsy/CLAUDE.md](https://github.com/Kochava-Studios/witsy/blob/c81c7de417a6362825bced2e865184d6e3fb73ba/CLAUDE.md) · 1981★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Witsy AI Assistant - Developer Guide

## Project Overview

Witsy is a cross-platform Electron-based desktop AI assistant that serves as a universal MCP (Model Context Protocol) client. Built with Electron, TypeScript, Vue 3, and Vite, it integrates multiple LLM providers and supports features like chat completion, image generation, speech-to-text, text-to-speech, document search (RAG), and automation capabilities.

## Architecture & Key Components

### Core Structure
- **Main Process** (`src/main/`): Electron main process handling system integration, IPC, and native APIs
- **Renderer Process** (`src/renderer`): Vue 3 frontend with Vite bundling 
- **Preload Scripts** (`src/preload.ts`): Secure IPC bridge between main and renderer
- **LLM Integration** (`src/renderer/services/llms/`): Multi-provider LLM abstraction layer using `multi-llm-ts`
- **Plugin System** (`src/renderer/services/plugins/`): Extensible tools for search, filesystem, python execution, etc.
- **Automation** (`src/main/automations/`): Cross-platform automation for "Prompt Anywhere" and AI commands

### Build System (Electron Forge + Vite)
- **Development**: `npm start` - runs with hot reload
- **Testing**: `npm t
```

</details>
