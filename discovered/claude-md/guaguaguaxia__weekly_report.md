---
name: guaguaguaxia__weekly_report
source: https://github.com/guaguaguaxia/weekly_report/blob/5b95c75867f434bfbca683341f21f1ddfb21fa1f/CLAUDE.md
repo: guaguaguaxia/weekly_report
kind: claude-md
stars: 3238
last_pushed: 2025-08-29T03:42:20Z
license: unknown
score: 7
domains: [web-frontend, ai-integration, nextjs]
tags: [architecture, nextjs, ai-prompting]
curated: 2026-06-15
curated_by: config-scout
---

# guaguaguaxia/weekly_report — claude-md

**Why it's worth keeping:** The 'Development Notes' section captures crucial hardcoded values like prompt strings and model parameters that are easily missed by agents scanning code.

**Summary:** Provides a clear architectural map of a Next.js application including component roles and specific AI integration details.

**Source credibility:** High star count (3k+) indicates a popular/widely used repository.

**Recency:** Current; aligns with modern Next.js and AI integration patterns.

**Source:** [guaguaguaxia/weekly_report/CLAUDE.md](https://github.com/guaguaguaxia/weekly_report/blob/5b95c75867f434bfbca683341f21f1ddfb21fa1f/CLAUDE.md) · 3238★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Next.js application that generates weekly reports using AI. Users input brief work descriptions and receive formatted weekly reports in markdown format. The application supports both Chinese and English localization and can use either server-side API keys or user-provided API keys.

## Commands

### Development
- `npm run dev` - Start development server on localhost:3000
- `npm run build` - Build the application for production
- `npm start` - Start production server

### Installation
- `npm install` - Install dependencies

## Architecture

### Core Components
- **Main UI**: `pages/index.tsx` - Main application interface with form inputs, loading states, and result display
- **API Handler**: `pages/api/generate.ts` - Edge function that processes requests and communicates with AI API
- **AI Streaming**: `utils/OpenAIStream.ts` - Handles streaming responses from DeepSeek API (not OpenAI despite the name)

### Key Features
- **Internationalization**: Uses next-intl with messages in `messages/` (en.json, zh.json)
- **AI Integration**: Curren
```

</details>
