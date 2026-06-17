---
name: antgroup__agentic-ai-landscape
source: https://github.com/antgroup/agentic-ai-landscape/blob/997fec7229a444a87d0e3210084398a3ed857ff7/CLAUDE.md
repo: antgroup/agentic-ai-landscape
kind: claude-md
stars: 496
last_pushed: 2026-06-02T09:10:48Z
license: unknown
score: 9
domains: [data-science, ai-analysis, python]
tags: [notebooks, data-pipeline, api-integration, workflow]
curated: 2026-06-15
curated_by: config-scout
---

# antgroup/agentic-ai-landscape — claude-md

**Why it's worth keeping:** Excellent documentation of the sequential 'Data Processing Pipeline' and specific 'Common Development Tasks,' enabling an agent to execute multi-step workflows autonomously. Includes critical API rate limits and endpoint details.

**Summary:** Provides an operational manual for a complex data analysis pipeline involving Jupyter notebooks, ClickHouse, and GitHub APIs.

**Source credibility:** High; produced by Ant Group with a highly active, well-maintained repository.

**Recency:** Extremely current, matching modern development environments and tool-use capabilities.

**Source:** [antgroup/agentic-ai-landscape/CLAUDE.md](https://github.com/antgroup/agentic-ai-landscape/blob/997fec7229a444a87d0e3210084398a3ed857ff7/CLAUDE.md) · 496★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This repository analyzes the **Open Source LLM Development Landscape** by tracking project vitality, trends, and community engagement metrics. The project uses [OpenRank](https://open-digger.cn/en/docs/user_docs/metrics/openrank) to assess repository health and identifies emerging trends in the LLM ecosystem. Reports are published on Medium and WeChat, with an interactive version on Canva.

## Environment Setup

### Prerequisites
- Python 3.12
- pip or conda for package management
- Access to ClickHouse database (credentials in `.env`)
- GitHub API token (for GitHub API calls)

### Initial Setup

1. **Create and activate virtual environment**:
   ```bash
   python3 -m venv .venv
   source .venv/bin/activate  # On macOS/Linux
   # or: .venv\Scripts\activate  # On Windows
   ```

2. **Configure environment variables** (`.env` file in `notebooks/` directory):
   ```
   GITHUB_TOKEN=your_github_token
   CLICKHOUSE_HOST=your_clickhouse_host
   CLICKHOUSE_USER=your_username
   CLICKHOUSE_PASSWORD=your_password
   HF_TOKEN=your_huggingface_token  # Opti
```

</details>
