---
name: wybert__earth-agent-chrome-ext
source: https://github.com/wybert/earth-agent-chrome-ext/blob/8b33aa0b7e96f837d10058d29f69b7a9dd61cf77/CLAUDE.md
repo: wybert/earth-agent-chrome-ext
kind: claude-md
stars: 104
last_pushed: 2026-04-27T02:27:36Z
license: mit
score: 8
domains: [chrome-extension, mcp-server, ai-agents, web-automation]
tags: [mcp, architecture-diagrams, workflow-constraints]
curated: 2026-06-15
curated_by: config-scout
---

# wybert/earth-agent-chrome-ext — claude-md

**Why it's worth keeping:** Includes a high-signal architectural flow diagram of the MCP/WebSocket/Service Worker relationship and strict 'negative constraints' regarding file organization and Git behavior.

**Summary:** Provides comprehensive context for a specialized MCP-to-Chrome-Extension bridge, detailing the unique communication architecture.

**Source credibility:** Solid mid-sized project (104 stars) with very recent maintenance activity.

**Recency:** Extremely current; focuses heavily on MCP protocols which are essential for modern Claude Code workflows.

**Source:** [wybert/earth-agent-chrome-ext/CLAUDE.md](https://github.com/wybert/earth-agent-chrome-ext/blob/8b33aa0b7e96f837d10058d29f69b7a9dd61cf77/CLAUDE.md) · 104★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

Guidance for Claude Code and other AI coding agents (Gemini, Cursor, Codex, etc.) working with this repository.

## Project Overview

Earth Agent is a Chrome extension (Manifest V3) + MCP server for Google Earth Engine. It enables AI-powered GEE automation through chat - write code, run analysis, debug errors, explain maps. Works as a Chrome extension or via MCP with Claude Code/Cursor.

## Quick Commands

```bash
npm run build          # Build extension to dist/
npm run format         # Format the code with Prettier
npm run dev            # Watch mode for development
npm run type-check     # TypeScript check
npm test               # Run Jest tests
```

## Version Management

```bash
npm version patch      # Bump version (auto-syncs all files)
git push --follow-tags # Triggers GitHub Actions release
cd mcp-server && npm publish  # Publish MCP to npm
```

Version synced across: `package.json`, `src/manifest.json`, `mcp-server/package.json`

## Project Structure

```
src/
├── background/        # Service worker, AI chat handler, MCP client
├── content/           # Earth Engine DOM manipulation
├── sidepanel/         # React UI
├── components/        # React components (C
```

</details>
