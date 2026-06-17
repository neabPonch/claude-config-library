---
name: rvdleun__rss-feeds-to-podcast
source: https://github.com/rvdleun/rss-feeds-to-podcast/blob/eaf098289f4e542942dbdcbe3c02a181f6ec3a55/CLAUDE.md
repo: rvdleun/rss-feeds-to-podcast
kind: claude-md
stars: 10
last_pushed: 2026-06-02T22:08:54Z
license: apache-2.0
score: 9
domains: [cli-tools, data-pipeline, backend-api]
tags: [nestjs, typescript, workflow-driven, media-processing]
curated: 2026-06-15
curated_by: config-scout
---

# rvdleun/rss-feeds-to-podcast — claude-md

**Why it's worth keeping:** The explicit description of the 7-step pipeline allows Claude to understand state transitions in a sequential process. Detailing the Zod configuration schema and the file-based dependency chain is highly effective for maintaining system integrity.

**Summary:** Provides clear CLI commands and a detailed breakdown of a multi-stage data processing workflow. It explains how the system moves from RSS retrieval through several LLM/TTS stages to final audio generation.

**Source credibility:** Reasonable; 10 stars and very recent activity indicates a stable, active project.

**Recency:** Very current; uses modern Node.js requirements and contemporary LLM/TTS service patterns.

**Source:** [rvdleun/rss-feeds-to-podcast/CLAUDE.md](https://github.com/rvdleun/rss-feeds-to-podcast/blob/eaf098289f4e542942dbdcbe3c02a181f6ec3a55/CLAUDE.md) · 10★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

### Building and Running
- `npm run build` - Build the project using NestJS CLI
- `npm run start` - Build and run the application (equivalent to `npm run build && node dist/main.js`)
- `node dist/main.js` - Run the built application directly
- `npm run start -- -Y` - Run with confirmation skip flag

### Testing and Quality
- `npm test` - Run Jest tests
- `npm run test:watch` - Run Jest tests in watch mode
- `npm run lint` - Run ESLint with auto-fix

### Project Management
- `npm run backlog` - Open the backlog browser for task management

## Architecture Overview

This is a **NestJS CLI application** that converts RSS feeds to podcast episodes using a multi-stage pipeline. The project uses:

- **NestJS Framework** with `nest-commander` for CLI functionality
- **TypeScript** with ES2021 target
- **Jest** for testing
- **ESLint** with Prettier for code quality
- **Zod** for configuration schema validation
- **External services**: LLM (OpenAI-compatible), Text-to-Speech (Kokoro), Web Scraper

### Key Structure
- `src/rss-feeds-to-podcast/` - Mai
```

</details>
