---
name: Chorus-AIDLC__Chorus
source: https://github.com/Chorus-AIDLC/Chorus/blob/6b7aae8f9ce057dafcc61d298f195862a1360b62/CLAUDE.md
repo: Chorus-AIDLC/Chorus
kind: claude-md
stars: 995
last_pushed: 2026-06-15T05:41:08Z
license: agpl-3.0
score: 9
domains: [fullstack-web, ai-agents, mcp-servers, backend-architecture]
tags: [nextjs, typescript, prisma, mcp, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# Chorus-AIDLC/Chorus — claude-md

**Why it's worth keeping:** It provides explicit rules on data identification (UUID-first), logic placement (Service Layer), and mandatory post-schema steps, preventing common LLM hallucinations in development. It also contains deep context on a custom permissioning system essential for the project's MCP tools.

**Summary:** A high-density technical blueprint that defines architectural constraints and operational workflows for an AI-driven full-stack application.

**Source credibility:** High; based on an active, highly-starred repository focused on AI/Human collaboration.

**Recency:** Very current, featuring cutting-edge versions like Next.js 15 and React 19.

**Source:** [Chorus-AIDLC/Chorus/CLAUDE.md](https://github.com/Chorus-AIDLC/Chorus/blob/6b7aae8f9ce057dafcc61d298f195862a1360b62/CLAUDE.md) · 995★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — Chorus Project Guide

## What is Chorus

Chorus is an AI Agent & Human collaboration platform implementing the **AI-DLC (AI-Driven Development Lifecycle)** workflow. AI Agents (with fine-grained, configurable permissions) and humans work together through a shared Idea → Proposal → Document + Task → Execute → Verify → Done pipeline.

Core philosophy: **"Reversed Conversation"** — AI proposes, humans verify (not human prompt → AI execute).

## Tech Stack

- **Framework**: Next.js 15 (App Router, Turbopack for dev)
- **Language**: TypeScript 5 (strict mode)
- **Frontend**: React 19, Tailwind CSS 4, shadcn/ui (Radix UI)
- **Database**: PostgreSQL 16, Prisma ORM 7
- **Cache/Pub-Sub**: Redis 7 (ioredis, optional — falls back to in-memory)
- **Testing**: Vitest 4
- **Auth**: OIDC (users), API Keys with `cho_` prefix (agents), SuperAdmin (env-based bcrypt)
- **MCP**: @modelcontextprotocol/sdk 1.26 (HTTP Streamable Transport)
- **i18n**: next-intl (en, zh)
- **Package Manager**: pnpm 9.15
- **Path alias**: `@/*` → `./src/*`

## Project Structure

```
src/
├── app/                    # Next.js App Router
│   ├── (dashboard)/        # Main app layout (sidebar nav)
│   │   ├── pr
```

</details>
