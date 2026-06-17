---
name: Droniu__saleor-stytch-integration-example
source: https://github.com/Droniu/saleor-stytch-integration-example/blob/1b2621b1a6d000420da0a6d8edfd3abd741f3639/Claude.md
repo: Droniu/saleor-stytch-integration-example
kind: claude-md
stars: 0
last_pushed: 2025-12-17T15:29:13Z
license: mit
score: 8
domains: [web-frontend, backend-api, auth-integration]
tags: [architecture-mapping, mcp-setup, dev-workflow]
curated: 2026-06-16
curated_by: config-scout
---

# Droniu/saleor-stytch-integration-example — claude-md

**Why it's worth keeping:** The 'Key Components' section maps file paths to their purpose—a high-value pattern for LLM context—and includes proactive MCP server installation commands.

**Summary:** Provides a comprehensive architectural map that links specific files to their functional responsibilities and outlines critical third-party configuration requirements.

**Source credibility:** Low; it is an unstarred example/fork repository.

**Recency:** Current; uses modern Claude Code MCP command syntax.

**Source:** [Droniu/saleor-stytch-integration-example/Claude.md](https://github.com/Droniu/saleor-stytch-integration-example/blob/1b2621b1a6d000420da0a6d8edfd3abd741f3639/Claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.
See Agents.md for additional content.

## Development Commands

- `npm install` - Install dependencies
- `npm start` or `npm run dev` - Start both frontend (port 3000) and backend (port 3001) concurrently
- `npm run build` - Build the application for production using Vite
- `npm run server` - Alternative command that also starts both frontend and backend

## Architecture Overview

This is a Stytch authentication example application built with React + TypeScript + Vite, demonstrating Email Magic Links and OAuth integration.

### Project Structure
- **Frontend**: React application using Vite dev server on port 3000
- **Backend**: Express.js server on port 3001 with authentication middleware
- **Authentication**: Stytch SDK for React with pre-built UI components

### Key Components

**Original Components:**
- `src/App.tsx` - Main router with conditional rendering based on user state
- `src/components/Login.tsx` - Handles authentication flow (extended with OIDC button)
- `src/components/Profile.tsx` - User profile display for authenticated users (extended with Saleor link
```

</details>
