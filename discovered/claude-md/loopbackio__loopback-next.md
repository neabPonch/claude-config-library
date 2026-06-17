---
name: loopbackio__loopback-next
source: https://github.com/loopbackio/loopback-next/blob/945a39297882ccdb65953fb72efebb4f6ce2a132/CLAUDE.md
repo: loopbackio/loopback-next
kind: claude-md
stars: 5095
last_pushed: 2026-06-14T21:08:21Z
license: other
score: 9
domains: [backend, nodejs, typescript]
tags: [monorepo, architecture, api]
curated: 2026-06-15
curated_by: config-scout
---

# loopbackio/loopback-next — claude-md

**Why it's worth keeping:** It includes critical 'Architectural Concepts' to prevent dependency errors and provides technical 'gotchas' (like the Lerna connector resolution issue) that would otherwise cause AI hallucinations.

**Summary:** A highly detailed guide for a complex TypeScript monorepo, covering build workflows, architectural patterns, and specific development constraints.

**Source credibility:** High; LoopBack is a mature, widely-used enterprise framework with significant community traction.

**Recency:** Highly relevant for modern TypeScript/Node.js development and Claude Code workflows.

**Source:** [loopbackio/loopback-next/CLAUDE.md](https://github.com/loopbackio/loopback-next/blob/945a39297882ccdb65953fb72efebb4f6ce2a132/CLAUDE.md) · 5095★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with
code in this repository.

## Project Overview

LoopBack 4 is a highly extensible Node.js and TypeScript framework for building
APIs and microservices. This is the monorepo (`loopback-next`) containing all
core packages, extensions, and examples.

## Monorepo Structure

- **packages/** — Core framework packages (~29 packages)
- **extensions/** — Optional extensions (authentication-jwt, graphql, cron,
  metrics, logging, etc.)
- **examples/** — Sample applications demonstrating features
- **acceptance/** — Database connector acceptance tests
- **fixtures/** — Test fixtures and mock services
- **bodyparsers/** — Body parser extensions
- **sandbox/** — For testing monorepo packages as local dependencies
- **benchmark/** — Performance benchmarks
- **docs/** — Jekyll-based documentation site

Managed with **Lerna** (independent versioning) and **npm workspaces**.

## Build & Development Commands

```bash
# Install dependencies (also auto-updates TypeScript project references)
npm ci

# Build all packages (incremental TypeScript compilation)
npm run build

# Full clean rebuild
npm run clean && npm r
```

</details>
