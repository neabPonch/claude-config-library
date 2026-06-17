---
name: davila7__claude-code-templates__claude
source: https://github.com/davila7/claude-code-templates/blob/6772ba97d5b016c87f70610429c7c44df934cfe1/docs/CLAUDE.md
repo: davila7/claude-code-templates
kind: claude-md
stars: 28060
last_pushed: 2026-06-15T04:33:54Z
license: mit
score: 9
domains: [web-frontend, cli-tools]
tags: [architecture-heavy, workflow-driven]
curated: 2026-06-15
curated_by: config-scout
---

# davila7/claude-code-templates — claude-md

**Why it's worth keeping:** Uses explicit code-pattern examples as ground truth and maps out multi-stage generation pipelines that an AI can follow to update the project.

**Summary:** Provides comprehensive architectural context, data schemas, and deployment workflows for a component marketplace.

**Source credibility:** Highly credible; high star count and active maintenance record.

**Recency:** Current; specifically optimized for modern Claude Code component workflows.

**Source:** [davila7/claude-code-templates/docs/CLAUDE.md](https://github.com/davila7/claude-code-templates/blob/6772ba97d5b016c87f70610429c7c44df934cfe1/docs/CLAUDE.md) · 28060★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This directory contains the static website (aitmpl.com) that serves as the public web interface for browsing and installing Claude Code components. The site is a vanilla JavaScript application that loads component data dynamically and provides an interactive browsing experience for 500+ components including agents, commands, settings, hooks, MCPs, and templates.

## Development Commands

### Local Development
```bash
# Serve locally with any static file server
python -m http.server 8000
# or
npx http-server

# Open browser to http://localhost:8000
```

### Component Data Generation
```bash
# From project root - regenerate components.json
cd ..
python scripts/generate_components_json.py

# This creates/updates docs/components.json with all components
```

### Deployment
- Site is automatically deployed to GitHub Pages when changes are pushed to `docs/` directory
- Deployed at: https://aitmpl.com (davila7.github.io/claude-code-templates)
- Vercel configuration in `vercel.json` for routing

## Architecture

### Data Flow
1. **Component Generation**:
```

</details>
