---
name: yy4382__tts-importer
source: https://github.com/yy4382/tts-importer/blob/552eb7d4ce0f6b68f77249b0770f394764b54d24/CLAUDE.md
repo: yy4382/tts-importer
kind: claude-md
stars: 421
last_pushed: 2026-05-31T13:56:10Z
license: unknown
score: 8
domains: [web-frontend, configuration-tools]
tags: [nextjs, zod, testing-patterns, state-management]
curated: 2026-06-15
curated_by: config-scout
---

# yy4382/tts-importer — claude-md

**Why it's worth keeping:** It includes a 'Key Patterns' section with concrete code snippets for testing complex state transitions with Immer, providing the AI with exact logic templates rather than vague instructions.

**Summary:** A guide for a Next.js project that converts Azure TTS configurations into various reading app formats using Zod and Jotai.

**Source credibility:** The repository is well-starred (421) and shows very recent activity.

**Recency:** Very current, specifically referencing Next.js 15 and modern development workflows.

**Source:** [yy4382/tts-importer/CLAUDE.md](https://github.com/yy4382/tts-importer/blob/552eb7d4ce0f6b68f77249b0770f394764b54d24/CLAUDE.md) · 421★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

- **Build**: `pnpm build` - Build the Next.js application
- **Development**: `pnpm dev` - Run development server with Turbopack
- **Lint**: `pnpm lint` - Run Next.js linting
- **Test all**: `pnpm test` - Run all Vitest tests
- **Test single file**: `pnpm vitest run <file-path>` - Run specific test file
- **Type check**: `pnpm tsc --noEmit` - Check TypeScript types without emitting files

## Project Architecture

This is a Next.js 15 application that generates configuration files for Azure TTS (Text-to-Speech) integration with various Chinese reading applications like Legado, iFreetime, and Read Aloud.

### Core Structure

**State Management**: Uses Jotai for global state management, particularly for Azure TTS configuration state defined in `src/lib/azure/schema.ts`.

**Azure TTS Integration** (`src/lib/azure/`):
- `schema.ts` - Core Zod schemas for Azure TTS configuration including `azureStateSchema`, `voiceConfigSchema`, and `speakerSchema`
- `config-to-url.ts` - Bidirectional conversion between Azure state objects and URL parameters using Z
```

</details>
