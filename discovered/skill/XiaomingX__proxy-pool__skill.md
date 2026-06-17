---
name: XiaomingX__proxy-pool__skill
source: https://github.com/XiaomingX/proxy-pool/blob/b25de0c06acb4f78995bf20bfc97ca036304dd1b/.prompt/skill.md
repo: XiaomingX/proxy-pool
kind: skill
stars: 133
last_pushed: 2026-03-08T02:55:59Z
license: apache-2.0
score: 8
domains: [backend-api, python, tooling]
tags: [architecture, asyncio, system-design]
curated: 2026-06-15
curated_by: config-scout
---

# XiaomingX/proxy-pool — skill

**Why it's worth keeping:** Includes highly transferable patterns for weighted scoring logic, semaphore-based concurrency control, and UX-centric API design (round-robin/multi-format).

**Summary:** A high-density architectural blueprint for building resilient asynchronous services and specialized management tools.

**Source credibility:** Based on a functional Python utility with moderate community traction.

**Recency:** Very current; utilizes modern standards like `uv` for project management.

**Source:** [XiaomingX/proxy-pool/.prompt/skill.md](https://github.com/XiaomingX/proxy-pool/blob/b25de0c06acb4f78995bf20bfc97ca036304dd1b/.prompt/skill.md) · 133★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Skills & Capabilities

## Skill 1: Modern Project Setup (uv-based project construction)
**Goal:** Create a modern Python project with environment isolation and clear dependencies.
**Actionable Steps:**
1.  **Initialization:** Use `uv init` to initialize the project structure and generate `pyproject.toml`.
2.  **Dependency Management:** Use `uv add fastapi uvicorn[standard] aiohttp apscheduler redis pydantic-settings loguru` to add core dependencies.
3.  **Development Environment:** Configure `.python-version` to lock the Python version, ensuring consistency in team collaboration.

## Skill 2: Core Logic Implementation (Collection & Intelligent Scoring)
**Goal:** Establish a dynamic proxy pool maintenance mechanism based on scores.
**Actionable Steps:**
1.  **Asynchronous Fetcher:** Define `BaseFetcher` and implement multi-source asynchronous crawling.
2.  **Weighted Scoring System:**
    -   Initial Score: 10
    -   Successful Verification: +10 (max 100)
    -   Failed Verification: -20 (min 0, delete if it reaches 0)
    -   *Purpose:* Only extremely stable proxies are retained long-term.
3.  **Concurrent Verification:** Use `asyncio.Semaphore` to limit the number of concurrent
```

</details>
