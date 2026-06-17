---
name: yokingma__SearChat
source: https://github.com/yokingma/SearChat/blob/7423e2cb092193e5947ed8650f8df095b2434b3e/CLAUDE.md
repo: yokingma/SearChat
kind: claude-md
stars: 1050
last_pushed: 2026-05-13T10:20:24Z
license: mit
score: 8
domains: [monorepo, fullstack-web, ai-agents]
tags: [turborepo, node-backend, vue-frontend, workspace-management]
curated: 2026-06-15
curated_by: config-scout
---

# yokingma/SearChat — claude-md

**Why it's worth keeping:** It teaches an AI how to navigate a workspace by explicitly linking specific directories to their unique development workflows and entry points.

**Summary:** A highly structured monorepo guide that defines architecture, granular commands for sub-apps, and critical configuration details.

**Source credibility:** High; the repository is popular (1050+ stars) and actively maintained.

**Recency:** Current; uses modern tooling like Turborepo, Vite, and Vue 3.

**Source:** [yokingma/SearChat/CLAUDE.md](https://github.com/yokingma/SearChat/blob/7423e2cb092193e5947ed8650f8df095b2434b3e/CLAUDE.md) · 1050★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is "Open AI Search" - a conversation-based search application with LLM support that includes Deep Research capabilities. It's built as a monorepo using Turborepo with two main applications: a Node.js/Koa backend server and a Vue.js frontend.

## Architecture

### Monorepo Structure
- **Root**: Turborepo workspace with yarn@3.5.1 package manager
- **apps/server**: Node.js backend (Koa.js framework, TypeScript)
- **apps/web**: Vue.js frontend (Vue 3, TypeScript, Vite, TDesign UI)

### Key Technologies
- **Backend**: Koa.js, TypeScript, LangChain, multiple LLM providers (OpenAI, Google, DeepSeek, etc.)
- **Frontend**: Vue 3, TypeScript, Vite, Pinia (state management), TDesign Vue Next, Tailwind CSS
- **Build System**: Turborepo for monorepo management
- **Search Engines**: SearXNG, Bing, Google, Tavily integration
- **AI Features**: Deep Research mode with iterative search and analysis

## Development Commands

### Root Level (Turborepo)
```bash
# Start development servers for both apps
turbo dev
# or
yarn dev

# Build all applications
turbo bu
```

</details>
