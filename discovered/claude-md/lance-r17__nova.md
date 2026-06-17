---
name: lance-r17__nova
source: https://github.com/lance-r17/nova/blob/b22a121a6745fc992fc0f5f420cd4ae764f102c8/CLAUDE.md
repo: lance-r17/nova
kind: claude-md
stars: 0
last_pushed: 2026-06-08T12:42:15Z
license: unknown
score: 9
domains: [web-frontend, backend-api, infrastructure-as-code]
tags: [full-stack, architectural-patterns, testing-standards, devops]
curated: 2026-06-16
curated_by: config-scout
---

# lance-r17/nova — claude-md

**Why it's worth keeping:** The inclusion of explicit testing file-naming standards and phase-based scope definitions is a top-tier technique for maintaining AI consistency. The detailed breakdown of the 'Metadata-Driven Dynamic Forms' pattern also helps the agent understand core business logic before touching code.

**Summary:** A highly structured technical manual that combines high-level architectural patterns with granular developer commands. It provides essential context for an LLM to understand system logic and maintain project consistency.

**Source credibility:** Low social proof on GitHub, but the technical depth suggests a sophisticated, well-engineered project.

**Recency:** Very recent; utilizes modern tooling like Python's `uv` and TailwindCSS v4.

**Source:** [lance-r17/nova/CLAUDE.md](https://github.com/lance-r17/nova/blob/b22a121a6745fc992fc0f5f420cd4ae764f102c8/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a **Nova** project designed to enable users to create compliant cloud resources across multiple cloud platforms through a unified web interface. The platform serves as a centralized hub for cloud infrastructure deployment with integrated compliance checking and real-time status tracking.

## Architecture Overview

### Full-Stack Architecture
- **Frontend**: React 18+ with TypeScript, using shadcn/ui components and TailwindCSS
- **Backend**: Python 3.11+ with FastAPI for async API development
- **Database**: PostgreSQL 15+ for all data persistence
- **Integration**: Apache Airflow for Infrastructure as Code (IaC) deployment execution
- **Authentication**: SSO integration with JWT tokens and role-based access control

### Key Architectural Patterns

#### Metadata-Driven Dynamic Forms
The platform uses a database-driven metadata system to generate dynamic forms for cloud resource configuration:
- Resource schemas stored in PostgreSQL as JSONB
- React JSON Schema Form generates UI components dynamically
- Parameter validation and dependencies
```

</details>
