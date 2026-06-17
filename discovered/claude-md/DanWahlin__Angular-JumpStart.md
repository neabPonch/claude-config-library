---
name: DanWahlin__Angular-JumpStart
source: https://github.com/DanWahlin/Angular-JumpStart/blob/bebc5431dfc65111a88bc2a5a27abf59888dd91d/CLAUDE.md
repo: DanWahlin/Angular-JumpStart
kind: claude-md
stars: 1593
last_pushed: 2026-02-14T10:06:32Z
license: mit
score: 9
domains: [web-frontend, fullstack]
tags: [command-timing, testing-flows, architecture-mapping]
curated: 2026-06-15
curated_by: config-scout
---

# DanWahlin/Angular-JumpStart — claude-md

**Why it's worth keeping:** The inclusion of estimated command durations (to prevent tool timeouts) and specific user-flow checklists for verification are elite, highly transferable techniques for AI agents.

**Summary:** A high-quality instruction file that includes critical execution timing for commands and explicit manual testing workflows.

**Source credibility:** High; a well-regarded repository with over 1500 stars and recent updates.

**Recency:** Very current; uses Angular 19 and was updated within the last few months.

**Source:** [DanWahlin/Angular-JumpStart/CLAUDE.md](https://github.com/DanWahlin/Angular-JumpStart/blob/bebc5431dfc65111a88bc2a5a27abf59888dd91d/CLAUDE.md) · 1593★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Angular JumpStart is an Angular 19 TypeScript application with a Node.js Express server backend that demonstrates key Angular concepts including routing, components, services, forms, and HTTP client usage. The project has been optimized with a custom CSS architecture using CSS Grid (Bootstrap-free) and utility classes for consistent design patterns.

## Essential Commands

### Development Workflow
```bash
# Install dependencies (takes ~40 seconds - set timeout to 90+ seconds)
npm install

# Development build (takes ~12 seconds - set timeout to 60+ seconds)
npx ng build angular-jumpstart --configuration development

# Start server (serves on http://localhost:8080)
npm start
```

### Docker Commands
```bash
# Build containers
docker-compose build node    # Node.js API container
docker-compose build nginx   # Nginx frontend container
docker-compose up           # Run complete containerized application
```

### Other Commands
```bash
# Cypress E2E tests (requires manual cypress installation first)
npm run cypress
npm run cypress:headless

# Storybook
```

</details>
