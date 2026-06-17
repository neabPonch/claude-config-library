---
name: Zedit42__clawdbot-skills__exa-skill
source: https://github.com/Zedit42/clawdbot-skills/blob/4b35c3f4ebec200b414afffae0382fef3c3fa19f/exa-SKILL.md
repo: Zedit42/clawdbot-skills
kind: skill
stars: 0
last_pushed: 2026-02-10T18:04:08Z
license: unknown
score: 7
domains: [agents-ai, cli-tools, web-search]
tags: [exa-api, semantic-search, research-tools]
curated: 2026-06-16
curated_by: config-scout
---

# Zedit42/clawdbot-skills — skill

**Why it's worth keeping:** It formalizes a critical agent workflow: finding specialized information (research papers/code) and then extracting the raw text for ingestion.

**Summary:** Integrates Exa AI to provide semantic web search and full-text content extraction via CLI scripts.

**Source credibility:** Low; the repository has zero stars and an unknown license.

**Recency:** Current; updated within the last 4 months.

**Source:** [Zedit42/clawdbot-skills/exa-SKILL.md](https://github.com/Zedit42/clawdbot-skills/blob/4b35c3f4ebec200b414afffae0382fef3c3fa19f/exa-SKILL.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: exa
description: Neural web search and code context via Exa AI API. Requires EXA_API_KEY. Use for finding documentation, code examples, research papers, or company info.
metadata: {"clawdbot":{"emoji":"🧠","requires":{"env":["EXA_API_KEY"]}}}
---

# Exa - Neural Web Search

Direct API access to Exa's neural search engine.

## Setup

**1. Get your API Key:**
Get a key from [Exa Dashboard](https://dashboard.exa.ai/api-keys).

**2. Set it in your environment:**
```bash
export EXA_API_KEY="your-key-here"
```

## Usage

### Web Search
```bash
bash scripts/search.sh "query" [num_results] [type]
```
*   `type`: auto (default), neural, fast, deep
*   `category`: company, research-paper, news, github, tweet, personal-site, pdf

### Code Context
Finds relevant code snippets and documentation.
```bash
bash scripts/code.sh "query" [num_results]
```

### Get Content
Extract full text from URLs.
```bash
bash scripts/content.sh "url1" "url2"
```
```

</details>
