---
name: joemckenney__website
source: https://github.com/joemckenney/website/blob/e57a67f5ed45b7be4580041074b9790758c46a93/CLAUDE.md
repo: joemckenney/website
kind: claude-md
stars: 0
last_pushed: 2026-05-12T17:32:10Z
license: unknown
score: 9
domains: [monorepo, fullstack, devops, backend-api]
tags: [typescript, k8s, turborepo, fastify, gitops]
curated: 2026-06-15
curated_by: config-scout
---

# joemckenney/website — claude-md

**Why it's worth keeping:** Provides specific procedural steps for scaling the architecture ('Adding a New Service') and details architectural exceptions like how streaming endpoints bypass the SDK pattern.

**Summary:** A comprehensive guide for a complex TypeScript monorepo that covers the full lifecycle from local development to Kubernetes deployment via GitOps.

**Source credibility:** Highly credible technical depth despite low star count; reflects professional-grade monorepo/DevOps patterns.

**Recency:** 

**Source:** [joemckenney/website/CLAUDE.md](https://github.com/joemckenney/website/blob/e57a67f5ed45b7be4580041074b9790758c46a93/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

A TypeScript monorepo with type-safe API generation, Kubernetes deployment, and observability. Self-hosted on k3s (rookery VM) with FluxCD GitOps and Cloudflare Tunnel ingress.

## Repository Structure

```
apps/
  www/                - Crowprose homepage (SSG): blog, projects, contributions
  dashboard/          - React + Vite chat client (multi-provider)

services/
  @gateway/
    service/          - Fastify API gateway: OAuth, JWT auth, proxy to @ai and @users
    sdk/              - Auto-generated TypeScript client from OpenAPI spec
    spec/             - OpenAPI specification package
  @users/
    service/          - User management Fastify API with Prisma
    db/               - Prisma ORM package (PostgreSQL)
    sdk/              - Auto-generated TypeScript client
    spec/             - OpenAPI specification package
  @ai/
    service/          - Multi-provider LLM chat backend (Vercel AI Gateway, Anthropic, Ollama)
    spec/             - OpenAPI specification package (no SDK — streaming endpoints aren't generated)
  @weather/
    serv
```

</details>
