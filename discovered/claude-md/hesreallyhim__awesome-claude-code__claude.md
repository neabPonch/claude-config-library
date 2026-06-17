---
name: hesreallyhim__awesome-claude-code__claude
source: https://github.com/hesreallyhim/awesome-claude-code/blob/614f102accbcd48206d63a21df64adc984026b40/resources/claude.md-files/SG-Cars-Trends-Backend/CLAUDE.md
repo: hesreallyhim/awesome-claude-code
kind: claude-md
stars: 46505
last_pushed: 2026-04-27T14:40:18Z
license: other
score: 9
domains: [fullstack, monorepo, devops]
tags: [monorepo-structure, mcp-documentation, command-catalog]
curated: 2026-06-15
curated_by: config-scout
---

# hesreallyhim/awesome-claude-code — claude-md

**Why it's worth keeping:** Demonstrates hierarchical configuration using directory-specific CLAUDE.md files and instructs the agent on using MCP tools to fetch external documentation.

**Summary:** A high-density guide for a full-stack monorepo that bridges the gap between codebase and architectural intent.

**Source credibility:** High; part of a majorly starred 'awesome' repository with recent activity.

**Recency:** Very current, referencing Next.js 15 and SST v3.

**Source:** [hesreallyhim/awesome-claude-code/resources/claude.md-files/SG-Cars-Trends-Backend/CLAUDE.md](https://github.com/hesreallyhim/awesome-claude-code/blob/614f102accbcd48206d63a21df64adc984026b40/resources/claude.md-files/SG-Cars-Trends-Backend/CLAUDE.md) · 46505★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Documentation Access

When working with external libraries or frameworks, use the Context7 MCP tools to get up-to-date documentation:

1. Use `mcp__context7__resolve-library-id` to find the correct library ID for any package
2. Use `mcp__context7__get-library-docs` to retrieve comprehensive documentation and examples

This ensures you have access to the latest API documentation for dependencies like Hono, Next.js, Drizzle ORM, Vitest,
and others used in this project.

# SG Cars Trends - Developer Reference Guide

## Project-Specific CLAUDE.md Files

This repository includes directory-specific CLAUDE.md files with detailed guidance for each component:

- **[apps/api/CLAUDE.md](apps/api/CLAUDE.md)**: API service development with Hono, workflows, tRPC, and social media integration
- **[apps/web/CLAUDE.md](apps/web/CLAUDE.md)**: Web application development with Next.js 15, HeroUI, blog features, and analytics
- **[packages/database/CLAUDE.md](packages/database/CLAUDE.md)**: Database schema management with Drizzle ORM, migrations, and TypeScript integration
- **[infra/
```

</details>
