---
name: FullAgent__fulling
source: https://github.com/FullAgent/fulling/blob/a524c5ec86518c8d415bcb949da6c81879bdb956/CLAUDE.md
repo: FullAgent/fulling
kind: claude-md
stars: 2422
last_pushed: 2026-05-22T06:47:21Z
license: mit
score: 9
domains: [full-stack, devops, infrastructure]
tags: [kubernetes, reconciliation-pattern, nextjs, architecture]
curated: 2026-06-14
curated_by: config-scout
---

# FullAgent/fulling — claude-md

**Why it's worth keeping:** It details the 'asynchronous reconciliation pattern' which prevents an AI from incorrectly attempting synchronous operations; it also includes specific naming patterns and file-to-function mappings essential for complex navigation.

**Summary:** This config provides deep architectural context for an asynchronous system managing Kubernetes resources via a Next.js backend. It explains the mental model of state reconciliation required to interact with the platform correctly.

**Source credibility:** High: 2.4k stars and active development as of last month.

**Recency:** Very current: references Next.js 16, React 19, and Tailwind v4.

**Source:** [FullAgent/fulling/CLAUDE.md](https://github.com/FullAgent/fulling/blob/a524c5ec86518c8d415bcb949da6c81879bdb956/CLAUDE.md) · 2422★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**Fulling v2** is an AI-powered development platform that integrates AI Agent ecosystem to provide full-stack development capabilities. Users can import existing projects from GitHub or create new projects directly on the platform.

**Core Value**: Free users' mental bandwidth through AI Agents. Users focus on development while Agents silently handle complex operations (deployment, infrastructure, etc.) without interruption.

**Key Features**:
- **Flexible Project Creation**: Import from GitHub repositories or create new projects from scratch
- **Optional Database**: Add PostgreSQL database on-demand when needed
- **AI Agent Ecosystem**: AI agents handle development, testing, deployment, and infrastructure management
- **Automated Operations**: Deployment, scaling, and infrastructure management happen automatically in the background
- **Full-Stack Development**: Complete environment with optional database, terminal, and file management
- **Zero Infrastructure Knowledge Required**: Users don't need to understand Kubernetes, networking, or DevOps
```

</details>
