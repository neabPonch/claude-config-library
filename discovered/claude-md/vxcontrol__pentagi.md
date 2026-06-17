---
name: vxcontrol__pentagi
source: https://github.com/vxcontrol/pentagi/blob/879e87c2c2688c4a95eac9c1aaf3cd6f6123ebe3/CLAUDE.md
repo: vxcontrol/pentagi
kind: claude-md
stars: 17728
last_pushed: 2026-06-13T12:02:21Z
license: mit
score: 9
domains: [backend-api, web-frontend, agents-ai, security]
tags: [monorepo, procedural-workflows, go, react]
curated: 2026-06-15
curated_by: config-scout
---

# vxcontrol/pentagi — claude-md

**Why it's worth keeping:** Includes 'Implementation Playbooks' for multi-step cross-package updates and explicitly links file modifications to required code-generation commands.

**Summary:** Provides a comprehensive architectural map of a complex monorepo alongside specific procedural workflows for system expansion.

**Source credibility:** High; based on a highly starred, active security-focused agentic platform.

**Recency:** Current; utilizes modern toolchains (pnpm, Go, Docker) and reflects contemporary AI development patterns.

**Source:** [vxcontrol/pentagi/CLAUDE.md](https://github.com/vxcontrol/pentagi/blob/879e87c2c2688c4a95eac9c1aaf3cd6f6123ebe3/CLAUDE.md) · 17728★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Core Interaction Rules

1. **Always use English** for all interactions, responses, explanations, and questions with users.
2. **Password Complexity Requirements**: For all password-related development (registration, password reset, API token generation, etc.), the following rules must be enforced:
   - Minimum 12 characters
   - Must contain at least 1 uppercase letter, 1 lowercase letter, 1 number, and 1 special character
   - Common weak passwords (e.g., `password`, `123456`) are prohibited
   - Both backend and frontend validation must be implemented; do not rely on frontend validation alone

## Project Overview

**PentAGI** is an automated security testing platform powered by AI agents. It runs autonomous penetration testing workflows using a multi-agent system (Researcher, Developer, Executor agents) that coordinates LLM providers, Docker-sandboxed tool execution, and a persistent vector memory store.

The application is a monorepo with:
- **`backend/`** — Go REST + GraphQL API server
- **`frontend/`** — React + TypeScript web UI
- **`observability/`** — Opti
```

</details>
