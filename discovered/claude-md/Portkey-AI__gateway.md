---
name: Portkey-AI__gateway
source: https://github.com/Portkey-AI/gateway/blob/669825cbe89ee51569918b8f78a9db486fd69dd4/CLAUDE.md
repo: Portkey-AI/gateway
kind: claude-md
stars: 12078
last_pushed: 2026-05-25T13:54:51Z
license: mit
score: 9
domains: [backend-api, ai-infrastructure]
tags: [typescript, hono, architecture-focused]
curated: 2026-06-15
curated_by: config-scout
---

# Portkey-AI/gateway — claude-md

**Why it's worth keeping:** It defines functional architecture (the middleware pipeline and provider interface) rather than just listing files, and includes critical operational details like test timeouts to prevent agent hang-ups.

**Summary:** A highly structured guide for a high-performance AI gateway that explains the mental model of the system alongside specific execution commands.

**Source credibility:** Very high; based on a major, highly-starred AI infrastructure repository with recent activity.

**Recency:** Current; follows modern standards for providing context to agentic coding tools.

**Source:** [Portkey-AI/gateway/CLAUDE.md](https://github.com/Portkey-AI/gateway/blob/669825cbe89ee51569918b8f78a9db486fd69dd4/CLAUDE.md) · 12078★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is the **Portkey AI Gateway** - a fast, reliable AI gateway that routes requests to 250+ LLMs with sub-1ms latency. It's built with Hono framework for TypeScript/JavaScript and can be deployed to multiple environments including Cloudflare Workers, Node.js servers, and Docker containers.

## Development Commands

### Core Development
- `npm run dev` - Start development server using Wrangler (Cloudflare Workers)
- `npm run dev:node` - Start development server using Node.js
- `npm run build` - Build the project for production
- `npm run build-plugins` - Build the plugin system

### Testing
- `npm run test:gateway` - Run tests for the main gateway code (src/)
- `npm run test:plugins` - Run tests for plugins
- `jest src/` - Run specific gateway tests
- `jest plugins/` - Run specific plugin tests

### Code Quality
- `npm run format` - Format code with Prettier
- `npm run format:check` - Check code formatting
- `npm run pretty` - Alternative format command

### Deployment
- `npm run deploy` - Deploy to Cloudflare Workers
- `npm run start:node` - St
```

</details>
