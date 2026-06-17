---
name: nibzard__awesome-agentic-patterns
source: https://github.com/nibzard/awesome-agentic-patterns/blob/50f446aadc72eedfe1f2bdeed5bcdbcce8353860/CLAUDE.md
repo: nibzard/awesome-agentic-patterns
kind: claude-md
stars: 4677
last_pushed: 2026-06-08T16:36:32Z
license: apache-2.0
score: 9
domains: [web-frontend, documentation, ai-agents]
tags: [astro, markdown-driven, data-pipeline]
curated: 2026-06-15
curated_by: config-scout
---

# nibzard/awesome-agentic-patterns — claude-md

**Why it's worth keeping:** Includes high-value specific constraints like exact Markdown spacing requirements and absolute path rules to prevent deployment errors. It also clearly explains the implicit build process/data sync requirement.

**Summary:** Provides comprehensive instructions for maintaining a pattern-driven documentation site, covering the data pipeline from Markdown to JSON.

**Source credibility:** High; based on a highly-starred, active community repository of agentic patterns.

**Recency:** Current; tailored specifically for Claude Code with modern tooling instructions.

**Source:** [nibzard/awesome-agentic-patterns/CLAUDE.md](https://github.com/nibzard/awesome-agentic-patterns/blob/50f446aadc72eedfe1f2bdeed5bcdbcce8353860/CLAUDE.md) · 4677★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a documentation website for "Awesome Agentic Patterns" - a curated catalogue of AI agent design patterns. It uses Astro (apps/web/) to generate a static documentation site that can be deployed to Vercel.

## Key Commands

> **NOTE:** This project uses **bun** as the package manager, not npm.

### Development Workflow
```bash
# Initial setup (run once)
npm install                            # Install Node.js dependencies

# Standard development cycle
npm run dev                            # Serve docs locally at http://localhost:4321

# Building and deployment
npm run build                          # Build static site to apps/web/dist/
vercel deploy                          # Deploy to Vercel (primary)
```

## Architecture

The project has a unique architecture where pattern documentation drives the entire site:

1. **Pattern Files** (`patterns/*.md`): Source of truth for all patterns
   - Must include YAML front-matter with: title, status, authors, category, tags
   - Content sections: Problem, Solution, Example (with Mermaid diagrams), R
```

</details>
