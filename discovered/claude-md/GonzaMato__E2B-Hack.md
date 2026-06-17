---
name: GonzaMato__E2B-Hack
source: https://github.com/GonzaMato/E2B-Hack/blob/b6f8037182e21604f5d3b94d68c6bafdee6cdeb5/claude.md
repo: GonzaMato/E2B-Hack
kind: claude-md
stars: 3
last_pushed: 2025-11-22T19:08:30Z
license: mit
score: 9
domains: [agents-ai, backend-api, web-frontend]
tags: [state-machine, api-documentation, architecture-blueprint]
curated: 2026-06-15
curated_by: config-scout
---

# GonzaMato/E2B-Hack — claude-md

**Why it's worth keeping:** It provides explicit architectural flows (state machine transitions) and request/response examples which allow Claude to reason about integration points rather than just guessing.

**Summary:** A high-density instruction file that explains the core state machine, service responsibilities, and detailed API contracts.

**Source credibility:** High; part of a specialized E2B-based agentic toolset.

**Recency:** Very current, using modern stacks like Groq, Vite, and E2B sandboxes.

**Source:** [GonzaMato/E2B-Hack/claude.md](https://github.com/GonzaMato/E2B-Hack/blob/b6f8037182e21604f5d3b94d68c6bafdee6cdeb5/claude.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

---

# Autonomous QA & Bug Triage Agent

## 🎯 Project Overview

**Autonomous QA & Bug Triage Agent** for MCP Hackathon: Transforms vague bug reports into fully-triaged GitHub issues with reproduction evidence in ~60 seconds.

**Architecture**: Express API (State Machine) → Groq LLM → E2B Sandbox → GitHub Issues + React Dashboard

**Key Stats**:
- ~2,500 lines of source code
- 7 core services + agent controller
- PostgreSQL persistent storage via Prisma ORM
- React frontend with GitHub integration
- State machine: INTAKE → CLASSIFY → ENRICH → REPRODUCE → CREATE_ISSUE → COMPLETED
- Fire-and-forget async API with polling pattern
- **Server-only**: HTTP API only (no CLI)

**Status**: ✅ **PRODUCTION READY**
- Compiles without errors
- Database configured and tested
- All endpoints functional
- Express server fully integrated
- Frontend dashboard with GitHub integration

---

## 🔧 Essential Commands

### Backend Development

```bash
# Install dependencies
npm install

# Start PostgreSQL (required)
docker-compose up -d

# Watch mode development (recommended)
npm run dev

#
```

</details>
