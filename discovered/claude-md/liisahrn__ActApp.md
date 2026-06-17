---
name: liisahrn__ActApp
source: https://github.com/liisahrn/ActApp/blob/03d071af945a902316aaaf2380348244cb676fb1/claude.md
repo: liisahrn/ActApp
kind: claude-md
stars: 1
last_pushed: 2026-05-28T14:48:12Z
license: unknown
score: 7
domains: [agents-ai, workflow-automation]
tags: [architecture-pattern, agentic-orchestration]
curated: 2026-06-16
curated_by: config-scout
---

# liisahrn/ActApp — claude-md

**Why it's worth keeping:** The instruction to favor existing tools and update workflows during failure creates a self-improving loop; the architectural hierarchy reduces probabilistic error rates.

**Summary:** Defines a 'WAT' (Workflows, Agents, Tools) architecture that separates high-level reasoning from deterministic script execution.

**Source credibility:** Low-signal repository (1 star).

**Recency:** Current; highly applicable to modern agentic coding workflows.

**Source:** [liisahrn/ActApp/claude.md](https://github.com/liisahrn/ActApp/blob/03d071af945a902316aaaf2380348244cb676fb1/claude.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Agent Instructions


You're working inside the **WAT framework** (Workflows, Agents, Tools). This architecture separates concerns so that probabilistic AI handles reasoning while deterministic code handles execution. That separation is what makes this system reliable.

## The WAT Architecture

**Leyer 1: Workflows (The Instructions)**
- Markdown SOPs stored in `workflows/`
- Each workflow defines the objective, required inputs, which tools to use, expected outputs, and how to handle edge cases
- Written in plain language, the same way you'd brief someone on your team


**Layer 2: Agents (The Decision-Maker)**
- This is your role. You're responsible for intelligent coordination.
- Read the relevant workflow, run tools in the correct sequence, handle failures gracefully, and ask clarifying questions when needed
- You connect intent to execution without trying to do everything yourself
- Example: If you need to pull data from a website, don't attempt it directly. Read `workflows/scrape_website.md`, figure out the required inputs, then execute
`tools/scrape_single_site.py`


**Layer 3: Tools (The Execution)**
- Python scripts in `tools/` that do the actual work
- API calls, data tran
```

</details>
