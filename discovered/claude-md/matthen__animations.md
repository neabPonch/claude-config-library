---
name: matthen__animations
source: https://github.com/matthen/animations/blob/a04f0c0e783a77baa6438fa8babaf6dafdcbc903/CLAUDE.md
repo: matthen/animations
kind: claude-md
stars: 49
last_pushed: 2026-03-02T20:55:02Z
license: mit
score: 9
domains: [web-frontend, graphics, mathematical-visualizations]
tags: [react, typescript, shaders, playwright, pnpm]
curated: 2026-06-15
curated_by: config-scout
---

# matthen/animations — claude-md

**Why it's worth keeping:** It includes proactive instructions for visual debugging via Playwright MCP and provides exact CLI command templates for scaffolding new components to prevent structural errors.

**Summary:** Guides Claude through a specialized workflow for creating React-based mathematical animations using specific graphics libraries and shader management.

**Source credibility:** Decent; 49 stars suggests a legitimate niche tool rather than a throwaway project.

**Recency:** Very current; utilizes modern agentic patterns like MCP integration.

**Source:** [matthen/animations/CLAUDE.md](https://github.com/matthen/animations/blob/a04f0c0e783a77baa6438fa8babaf6dafdcbc903/CLAUDE.md) · 49★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a React-based mathematical animations project that creates interactive visualizations. Each animation is implemented as a React component with parameter controls, playback, and export functionality.

## Key Commands

### Development
- `pnpm install` - Install dependencies
- `pnpm start` - Start development server on localhost:3000
- `pnpm build` - Build for production
- `pnpm new-animation` - Interactive script to create new animations

### Package Manager
This project uses **pnpm** (not npm). Always use `pnpm` commands.

## Collaborative Development

### Playwright Integration
Playwright is a useful way to work on animations with the user, as it allows you to see the screen through screenshots and interact with the running application. This enables you to:
- Visually inspect animations as they run
- Verify that changes produce the expected visual results
- Debug rendering issues by seeing what's actually displayed

The user can enable Playwright support with:
```bash
claude mcp add playwright npx '@playwright/mcp@latest'
```

## Architec
```

</details>
