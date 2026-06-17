---
name: nextify-limited__libra
source: https://github.com/nextify-limited/libra/blob/454e5c45fb5406e69d12f290b489236870f2beb0/CLAUDE.md
repo: nextify-limited/libra
kind: claude-md
stars: 1625
last_pushed: 2025-09-24T02:11:26Z
license: agpl-3.0
score: 9
domains: [monorepo, fullstack-web, cloud-infrastructure]
tags: [turborepo, bun, nextjs, cloudflare, drizzle]
curated: 2026-06-15
curated_by: config-scout
---

# nextify-limited/libra — claude-md

**Why it's worth keeping:** Provides explicit 'Key Development Patterns' which give the AI mental models of how services interact, plus detailed directory-specific commands to navigate a large codebase.

**Summary:** A comprehensive guide for a complex Turborepo monorepo that includes architecture tree, specific technology versions, and essential command workflows.

**Source credibility:** Highly credible; high star count (1625) indicates a significant and well-used open-source project.

**Recency:** 

**Source:** [nextify-limited/libra/CLAUDE.md](https://github.com/nextify-limited/libra/blob/454e5c45fb5406e69d12f290b489236870f2beb0/CLAUDE.md) · 1625★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Architecture Overview

Libra is an AI-powered web development platform built as a Turborepo monorepo targeting Cloudflare Workers infrastructure. The codebase follows a microservices architecture with shared packages for common functionality.

### Core Structure
```
libra/
├── apps/                          # Application services
│   ├── web/                       # Next.js 15 main application (React 19)
│   ├── builder/                   # Vite build service
│   ├── cdn/                       # Hono CDN service
│   ├── deploy/                    # Deployment service V2 (Cloudflare Queues)
│   ├── deploy-workflow/           # Deployment service V1 (Cloudflare Workflows)
│   ├── dispatcher/                # Request routing (Workers for Platforms)
│   ├── auth-studio/               # Authentication management console
│   ├── docs/                      # Documentation site (Next.js + FumaDocs)
│   ├── email/                     # Email service (React Email)
│   ├── screenshot/                # Screenshot service
│   └── vite-shadcn-template/      # Project template e
```

</details>
