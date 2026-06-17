---
name: diffbot__langchain-diffbot
source: https://github.com/diffbot/langchain-diffbot/blob/3a233fe6d223e27a93763cb0ac1ac294f7c8dd14/CLAUDE.md
repo: diffbot/langchain-diffbot
kind: claude-md
stars: 0
last_pushed: 2026-06-10T22:46:23Z
license: mit
score: 9
domains: [ai-agents, api-integrations, python]
tags: [architecture-rules, dev-workflow, llm-integration]
curated: 2026-06-16
curated_by: config-scout
---

# diffbot/langchain-diffbot — claude-md

**Why it's worth keeping:** Includes 'architectural decisions' that explain the *why* behind trade-offs (like native async vs. thread pools) and maps documentation ownership to prevent drift.

**Summary:** Provides deep architectural rationale, specific toolchain instructions, and strict configuration patterns for a LangChain integration.

**Source credibility:** High; originates from a professional API integration repository with clear development standards.

**Recency:** 

**Source:** [diffbot/langchain-diffbot/CLAUDE.md](https://github.com/diffbot/langchain-diffbot/blob/3a233fe6d223e27a93763cb0ac1ac294f7c8dd14/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# langchain-diffbot

LangChain integration package for the Diffbot APIs (Knowledge Graph, Extract, Web Search, NLP entities, Crawl, and the Diffbot LLM RAG endpoint).

## Stack

- **Build/deps**: `uv` (not Poetry/pip). `pyproject.toml` is PEP 621 with `hatchling` as the build backend. Dependency groups (`test`, `lint`, `typing`) are declared under `[dependency-groups]` and invoked via `uv run --group <name> ...`.
- **HTTP / Diffbot transport**: the official [`diffbot-python`](https://github.com/diffbot/diffbot-python) SDK. It wraps `httpx` under the hood, so `respx` continues to work for unit tests — mocks target the real upstream URLs (KG: `https://kg.diffbot.com/kg/v3/dql`, web search: `https://llm.diffbot.com/api/v1/web_search`, extract: `https://api.diffbot.com/v3/analyze`, ask: `https://llm.diffbot.com/rag/v1/chat/completions`, NLP: `https://nl.diffbot.com/v1/`, crawl: `https://api.diffbot.com/v3/crawl`, ontology: `https://kg.diffbot.com/kg/ontology`). `diffbot-python` is published on PyPI and resolved from there as a normal dependency (`diffbot-python>=0.1.0`); `langchain-core` / `langchain-tests` are still resolved during local dev from the sibling `../langchain/` checkout v
```

</details>
