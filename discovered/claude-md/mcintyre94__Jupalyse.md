---
name: mcintyre94__Jupalyse
source: https://github.com/mcintyre94/Jupalyse/blob/a995191620425e05dfdc2b878faf91dc8a0d0452/CLAUDE.md
repo: mcintyre94/Jupalyse
kind: claude-md
stars: 20
last_pushed: 2026-01-10T13:27:54Z
license: mit
score: 9
domains: [web-frontend, blockchain]
tags: [react, typescript, architecture, devops]
curated: 2026-06-15
curated_by: config-scout
---

# mcintyre94/Jupalyse — claude-md

**Why it's worth keeping:** It provides a 'Request Flow' section to prevent security/architectural errors and identifies heavy files to help an AI manage context limits. The inclusion of mandatory linting commands ensures consistent code quality during agentic edits.

**Summary:** A high-density technical blueprint covering architecture, data flow patterns, and specific local development workflows. It explicitly details the dual-server startup requirement for API and frontend synchronization.

**Source credibility:** Solid open-source project; well-documented and specialized in the Solana ecosystem.

**Recency:** Current; uses modern stacks including React 18 and Vite.

**Source:** [mcintyre94/Jupalyse/CLAUDE.md](https://github.com/mcintyre94/Jupalyse/blob/a995191620425e05dfdc2b878faf91dc8a0d0452/CLAUDE.md) · 20★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Jupalyse - AI Assistant Guide

## Project Overview

Jupalyse is a web-based analytics and tracking tool for Jupiter DCAs (Dollar Cost Averaging) on Solana. It helps users monitor, analyze, and download data from their Jupiter recurring and trigger orders for tax reporting and personal record-keeping.

**Key Features:**

- View all Jupiter DCAs for any Solana address
- Display all trades in an interactive, feature-rich table
- Download CSV data suitable for tax preparation
- Optional USD price fetching for comprehensive reporting
- **Privacy-first**: Runs entirely locally, user data never sent to external servers

**Live Site:** https://jupalyse.vercel.app

## Tech Stack

### Frontend

- **React 18.3.1** - Core UI framework
- **React Router 6.27.0** - Client-side routing with data loaders
- **Vite 5.4.8** - Build tool and dev server with fast HMR
- **TypeScript 5.5.3** - Strict type checking enabled
- **Mantine 7.13.3** - Component library with dark mode support
- **Tabler Icons React 3.19.0** - Icon library

### State Management & Data Fetching

- **React Query (TanStack Query) 5.62.0** - Server state management with caching
- **React Query Persist Client** - localStorage persist
```

</details>
