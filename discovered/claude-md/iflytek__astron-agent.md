---
name: iflytek__astron-agent
source: https://github.com/iflytek/astron-agent/blob/87b9fa51b44fc7bb4ef07cf38db2527f3ed5628a/CLAUDE.md
repo: iflytek/astron-agent
kind: claude-md
stars: 8559
last_pushed: 2026-06-11T14:45:14Z
license: apache-2.0
score: 9
domains: [backend-api, microservices, ai-agents, devops]
tags: [monorepo, behavioral-constraints, surgical-coding, workflow-automation]
curated: 2026-06-15
curated_by: config-scout
---

# iflytek/astron-agent — claude-md

**Why it's worth keeping:** The 'Behavioral Guidelines' section is elite, offering specific principles like 'Surgical Changes' and 'Simplicity First' that combat common LLM tendencies to refactor unrelated code or add unnecessary abstractions.

**Summary:** Provides a comprehensive structural map of a multi-language monorepo alongside high-level behavioral constraints to prevent LLM over-engineering.

**Source credibility:** High; large star count (8k+) and active maintenance suggest this is a production-grade professional project.

**Recency:** Very current; demonstrates advanced usage of Claude Code features like subagent skills for PRs and deployments.

**Source:** [iflytek/astron-agent/CLAUDE.md](https://github.com/iflytek/astron-agent/blob/87b9fa51b44fc7bb4ef07cf38db2527f3ed5628a/CLAUDE.md) · 8559★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## Project Overview

Astron Agent is an enterprise-grade Agentic Workflow development platform. It includes the console frontend and backend, multiple core microservices, a plugin system, and deployment and infrastructure configuration. The repository uses a multi-language, multi-module structure. The primary languages are TypeScript, Java, Python, and Go.

## Repository Structure

### Console

- `console/frontend`
  - React 18 + TypeScript + Vite frontend application
  - Responsible for the console UI, agent creation, chat interface, workflow visualization, model management, plugin marketplace, and related features
- `console/backend`
  - Java Spring Boot backend
  - Responsible for console REST APIs, SSE, authentication, management capabilities, and business aggregation
  - Main submodules:
    - `hub`
    - `toolkit`
    - `commons`

### Core Microservices

- `core/agent`
  - Python FastAPI service
  - Responsible for the agent execution engine, Chat/CoT/CoT Process Agent, plugin invocation, and session context handling
- `core/workflow`
  - Python FastAPI service
  - Responsible for workflow orchestration, execution, debugging, versioning, and event handling
- `cor
```

</details>
