---
name: hoangsonww__Customizable-AI-Chatbot
source: https://github.com/hoangsonww/Customizable-AI-Chatbot/blob/712825011e6f1aca3b3b6bb87861e5fc0c48d852/CLAUDE.md
repo: hoangsonww/Customizable-AI-Chatbot
kind: claude-md
stars: 21
last_pushed: 2026-06-15T00:34:29Z
license: other
score: 9
domains: [agents-ai, backend-api, rag]
tags: [nextjs, rag, hyde, openai, architectural-guide]
curated: 2026-06-15
curated_by: config-scout
---

# hoangsonww/Customizable-AI-Chatbot — claude-md

**Why it's worth keeping:** The configuration mapping tells the agent exactly which files impact specific behaviors, while the RAG/HyDE breakdown provides essential semantic context for debugging retrieval issues.

**Summary:** Provides a deep architectural blueprint explaining the 'why' behind complex logic like HyDE-based RAG and intention detection.

**Source credibility:** Moderate popularity (21 stars) with very recent maintenance activity.

**Recency:** Current; uses modern Next.js 14 patterns and contemporary AI orchestration techniques.

**Source:** [hoangsonww/Customizable-AI-Chatbot/CLAUDE.md](https://github.com/hoangsonww/Customizable-AI-Chatbot/blob/712825011e6f1aca3b3b6bb87861e5fc0c48d852/CLAUDE.md) · 21★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

### Essential Commands

```bash
# Development
npm run dev          # Start Next.js dev server on localhost:3000
make dev            # Alternative using Makefile

# Building
npm run build       # Build production bundle
make build          # Alternative using Makefile

# Testing
npm test            # Run test suite
make test           # Alternative using Makefile

# Linting & Formatting
npm run lint        # Run ESLint
npm run format      # Format code with Prettier

# Setup
make setup          # Initial project setup (clone, install deps, scaffold .env)

# Deployment
make deploy         # Deploy to Vercel

# Pinecone/RAG
make upsert         # Upsert documents to Pinecone for RAG

# Customization
make customize      # Interactive config for UI/identity/prompts
```

### Package Manager

This project uses **pnpm** (version 9.12.0) as specified in package.json. If you need to install dependencies:

```bash
pnpm install
```

## Architecture Overview

This is a **Next.js 14 App Router** application implementing a multi-provider AI chatbot with RAG
```

</details>
