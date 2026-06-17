---
name: kyeotic__full-stack-template
source: https://github.com/kyeotic/full-stack-template/blob/b2b959b7074ee6da07b4cce8b1541dc1946580eb/CLAUDE.md
repo: kyeotic/full-stack-template
kind: claude-md
stars: 0
last_pushed: 2026-04-02T16:04:15Z
license: mit
score: 9
domains: [fullstack, cloudflare-workers, typescript]
tags: [architectural-patterns, agentic-workflow, security-guardrails]
curated: 2026-06-15
curated_by: config-scout
---

# kyeotic/full-stack-template — claude-md

**Why it's worth keeping:** It introduces a 'thoughts/' directory workflow for agentic planning/tracking and includes crucial security guardrails against reading .env secrets into context.

**Summary:** A highly structured guide for a full-stack SolidJS and Cloudflare Workers application using hexagonal architecture.

**Source credibility:** Recent personal project demonstrating professional-grade architectural patterns like dependency injection and hexagonal structure.

**Recency:** Very current, utilizing modern tech like Tailwind v4 and specifically tailored instructions for Claude's agentic capabilities.

**Source:** [kyeotic/full-stack-template/CLAUDE.md](https://github.com/kyeotic/full-stack-template/blob/b2b959b7074ee6da07b4cce8b1541dc1946580eb/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

When working ALWAYS start by making a markdown plan in thoughts/ unless the user says "skip plan"

- If a plan markdown already exists, or is provided by the user, work from the existing document instead of making a new one
- As you work update the thought markdown with changes and progress
- If you change the system or architecture documented in THIS DOCUMENT, UPDATE IT

DO NOT READ the .env file, it contains secrets that should NEVER be in the claude context
They are part of the ENV VARs, so you can use them (WITHOUT READING THEM INTO CONTEXT)

## Commands

```bash
# Development
npm run dev              # Frontend (Vite :3000) + Backend (Wrangler :8787) in parallel
npm run dev:frontend     # Vite dev server only
npm run dev:backend      # Wrangler Workers dev server only

# Build & Deploy
npm run build            # Vite build → dist/client/
npm run deploy           # Build + wrangler deploy to Cloudflare
npm run deploy:worker    # Wrangler deploy only
npm run deploy:infra     # Terraform infrastructure deploy

# Type checking & Linting
npm run check            # st
```

</details>
