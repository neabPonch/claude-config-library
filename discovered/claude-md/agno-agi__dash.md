---
name: agno-agi__dash
source: https://github.com/agno-agi/dash/blob/dfcf2bedeb13ad78d10d6cdeabb309766f98075e/CLAUDE.md
repo: agno-agi/dash
kind: claude-md
stars: 2087
last_pushed: 2026-04-08T11:50:51Z
license: apache-2.0
score: 9
domains: [agents-ai, data-engineering, backend]
tags: [architecture, agentic-workflows, knowledge-base, data-modeling]
curated: 2026-06-15
curated_by: config-scout
---

# agno-agi/dash — claude-md

**Why it's worth keeping:** The inclusion of 'Key gotchas' (data quirks) and the clear mapping of dual-schema permission boundaries provide crucial reasoning context that raw code cannot easily convey.

**Summary:** Acts as both a technical manual and a domain knowledge base, detailing agent roles, schema permissions, and data nuances.

**Source credibility:** High; Agno is a well-regarded agent framework with significant social proof (2k+ stars).

**Recency:** Very current; utilizes modern tooling like `uv` and Python 3.12.

**Source:** [agno-agi/dash/CLAUDE.md](https://github.com/agno-agi/dash/blob/dfcf2bedeb13ad78d10d6cdeabb309766f98075e/CLAUDE.md) · 2087★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## Project Overview

Dash is a self-learning data agent that delivers **insights, not just SQL results**. It uses a team of specialists (Analyst + Engineer) coordinated by a leader to handle data queries and build computed data assets. Built on [Agno](https://docs.agno.com). Runs in Slack, the terminal, or the [AgentOS](https://os.agno.com) web UI.

## Structure

```
dash/
├── team.py               # Dash team (leader, coordinate mode)
├── settings.py            # Shared config (DB, model, knowledge bases, Slack)
├── instructions.py        # Instruction builders per agent role
├── paths.py               # Path constants
├── __main__.py            # CLI entry point (python -m dash)
├── agents/
│   ├── analyst.py         # SQL queries, data analysis, insights (read-only)
│   └── engineer.py        # Views, summary tables, computed data (dash schema)
├── context/               # Runtime prompt builders (reads knowledge/)
│   ├── semantic_model.py  # Table metadata → system prompt
│   └── business_rules.py  # Business rules → system prompt
└── tools/
    ├── build.py           # Tool assembly per agent role (schema boundaries)
    ├── introspect.py      # Runtime schema in
```

</details>
