---
name: xianshang33__llm-paper-daily__skill
source: https://github.com/xianshang33/llm-paper-daily/blob/73a5b351dd28c78289306beaaf0a640a998c01a9/skill/paper-daily/SKILL.md
repo: xianshang33/llm-paper-daily
kind: skill
stars: 1268
last_pushed: 2026-06-13T08:38:07Z
license: unknown
score: 8
domains: [agents-ai, cli-tools, data-curation]
tags: [arxiv, llm, automation]
curated: 2026-06-14
curated_by: config-scout
---

# xianshang33/llm-paper-daily — skill

**Why it's worth keeping:** It demonstrates a sophisticated heuristic-based ranking workflow (keyword > category > institution) and provides granular CLI commands for dry runs and testing.

**Summary:** Automates the discovery, ranking, and curation of arXiv papers focusing on LLMs and AI Agents.

**Source credibility:** High; the source repository is popular with very recent activity.

**Recency:** Current; follows modern agentic tool-use patterns.

**Source:** [xianshang33/llm-paper-daily/skill/paper-daily/SKILL.md](https://github.com/xianshang33/llm-paper-daily/blob/73a5b351dd28c78289306beaaf0a640a998c01a9/skill/paper-daily/SKILL.md) · 1268★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: paper-daily
description: Discover daily arXiv papers for LLM/Agent topics, rank candidates with keyword and institution filters, and prepare a small selected paper list for llm-paper-daily style workflows.
---

# Paper Daily

Use this skill when maintaining a daily LLM/Agent paper list from arXiv.

## Workflow

1. Discover candidates from arXiv by priority keywords: `Agent`, `Agents`, then `LLM`.
2. Query target categories such as `cs.AI`, `cs.CL`, `cs.LG`, `stat.ML`, `cs.SE`, and `cs.MA`.
3. Dedupe by normalized arXiv id without version suffix.
4. Filter obvious noise such as chemical/biological/contrast agents.
5. Rank candidates with:
   - keyword priority
   - title/abstract Agent or LLM signals
   - category signals
   - institution signals from QS Top 50 universities and known AI labs/companies
6. Select 3-5 papers for summarization and deterministic README rendering when enough ranked candidates are available; fewer papers are allowed only when filtered candidates are genuinely insufficient.

## Commands

Run a real arXiv dry-run for a UTC submitted date:

```bash
python3 skill/paper-daily/scripts/discover.py --date YYYY-MM-DD --select 5
```

Write JSON output:

``
```

</details>
