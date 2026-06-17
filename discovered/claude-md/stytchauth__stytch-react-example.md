---
name: stytchauth__stytch-react-example
source: https://github.com/stytchauth/stytch-react-example/blob/67557f9697c3f08d1d1361a37a08bb90b055999c/Claude.md
repo: stytchauth/stytch-react-example
kind: claude-md
stars: 51
last_pushed: 2026-03-12T16:47:47Z
license: mit
score: 7
domains: [web-frontend, backend-api, agents-ai, authentication]
tags: [react, stytch, mcp, auth]
curated: 2026-06-15
curated_by: config-scout
---

# stytchauth/stytch-react-example — claude-md

**Why it's worth keeping:** It demonstrates how to instruct an agent to install required MCP servers and provides specific external dashboard configurations necessary for the app to run.

**Summary:** Provides clear full-stack architecture and critical external service configuration requirements.

**Source credibility:** High; comes from a professional authentication provider (Stytch).

**Recency:** Very current, specifically referencing modern Claude MCP installation workflows.

**Source:** [stytchauth/stytch-react-example/Claude.md](https://github.com/stytchauth/stytch-react-example/blob/67557f9697c3f08d1d1361a37a08bb90b055999c/Claude.md) · 51★

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
- `src/App.tsx` - Main router with conditional rendering based on user state
- `src/components/Login.tsx` - Handles authentication flow
- `src/components/Profile.tsx` - User profile display for authenticated users
- `src/components/Authorize.tsx` - Connected Apps authorization component
- `src
```

</details>
