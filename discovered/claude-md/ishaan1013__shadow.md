---
name: ishaan1013__shadow
source: https://github.com/ishaan1013/shadow/blob/96e7b187951d66740dcd7d0bf3d5f94f5d09ed41/CLAUDE.md
repo: ishaan1013/shadow
kind: claude-md
stars: 1484
last_pushed: 2026-03-19T20:29:22Z
license: mit
score: 9
domains: [agents-ai, fullstack-web, monorepo]
tags: [architecture-guide, workflow-orchestration, tool-system]
curated: 2026-06-15
curated_by: config-scout
---

# ishaan1013/shadow — claude-md

**Why it's worth keeping:** It provides concrete command snippets for common tasks and explains high-level system lifecycles which helps agents understand execution context rather than just file contents.

**Summary:** Acts as a comprehensive technical manual for an AI agent to navigate and develop the Shadow platform. It maps out monorepo architecture, internal tool logic, and specific development workflows.

**Source credibility:** High; the repository is well-starred and reflects a sophisticated agentic platform.

**Recency:** Extremely current, utilizing bleeding-edge technologies like Next.js 15 and React 19.

**Source:** [ishaan1013/shadow/CLAUDE.md](https://github.com/ishaan1013/shadow/blob/96e7b187951d66740dcd7d0bf3d5f94f5d09ed41/CLAUDE.md) · 1484★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Shadow Development Guide for Claude Code

This guide provides comprehensive information for Claude Code development on the Shadow platform - a remote, autonomous coding agent with hardware-isolated execution environments.

## Platform Overview

Shadow is an AI coding platform that enables autonomous agents to work on GitHub repositories through real-time collaboration, semantic code search, and long-horizon task management. The platform provides both local and remote execution modes with enterprise-grade security.

### Core Architecture

**Monorepo Structure** (Turborepo managed):
- `apps/frontend/` - Next.js 15 + React 19 application with real-time chat interface
- `apps/server/` - Node.js orchestrator for LLM integration and WebSocket communication  
- `apps/sidecar/` - Express.js service for isolated file operations and command execution
- `packages/db/` - Prisma schema and PostgreSQL client
- `packages/types/` - Shared TypeScript type definitions
- `packages/command-security/` - Security utilities for command validation

**Dual Execution Modes**:
- **Local Mode**: Direct filesystem execution on host machine for development
- **Remote Mode**: Hardware-isolated execution in Kat
```

</details>
