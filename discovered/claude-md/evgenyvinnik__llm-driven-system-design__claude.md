---
name: evgenyvinnik__llm-driven-system-design__claude
source: https://github.com/evgenyvinnik/llm-driven-system-design/blob/a5367a33a6ec0faa0d4be386814419a7055524bf/web-crawler/CLAUDE.md
repo: evgenyvinnik/llm-driven-system-design
kind: claude-md
stars: 40
last_pushed: 2026-03-18T18:46:53Z
license: mit
score: 8
domains: [backend, system-design]
tags: [architecture-log, decision-record]
curated: 2026-06-15
curated_by: config-scout
---

# evgenyvinnik/llm-driven-system-design — claude-md

**Why it's worth keeping:** The 'Design Decisions Log' captures the 'why' behind technical choices, preventing the AI from suggesting previously rejected alternatives or violating established patterns.

**Summary:** A living development journal that tracks architectural decisions, technical trade-offs, and project roadmap progress.

**Source credibility:** Low star count but demonstrates high-quality implementation of an LLM-driven development workflow.

**Recency:** Very recent (3 months ago), highly relevant to modern agentic coding workflows.

**Source:** [evgenyvinnik/llm-driven-system-design/web-crawler/CLAUDE.md](https://github.com/evgenyvinnik/llm-driven-system-design/blob/a5367a33a6ec0faa0d4be386814419a7055524bf/web-crawler/CLAUDE.md) · 40★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Web Crawler - Development with Claude

## Project Context

This document tracks the development journey of implementing a distributed web crawling system for indexing the internet.

## Key Challenges to Explore

1. Distributed coordination
2. Duplicate detection
3. Crawl politeness
4. URL prioritization

## Development Phases

### Phase 1: Requirements and Design
*Completed*

**Completed:**
- Defined functional requirements (URL discovery, page fetching, content extraction, politeness)
- Established scale targets based on system-design-answer-fullstack.md
- Identified key technical constraints (robots.txt compliance, rate limiting)

### Phase 2: Initial Implementation
*In Progress*

**Completed items:**
- Set up project structure (backend, frontend, Docker configuration)
- Implemented URL frontier with priority queue (PostgreSQL + Redis)
- Created crawler workers with politeness (robots.txt, rate limiting)
- Built content storage and link extraction
- Implemented API endpoints for dashboard and admin
- Created frontend dashboard with React, Vite, TanStack Router, Zustand, Tailwind CSS
- Set up Docker Compose for both development and production

**Focus areas:**
- [x] Implement co
```

</details>
