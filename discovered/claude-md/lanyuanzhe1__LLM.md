---
name: lanyuanzhe1__LLM
source: https://github.com/lanyuanzhe1/LLM/blob/142ae574a2137c715169c692c97d32759f108cd2/CLAUDE.md
repo: lanyuanzhe1/LLM
kind: claude-md
stars: 0
last_pushed: 2026-06-16T09:03:08Z
license: unknown
score: 8
domains: [agents-ai, rag-pipeline, backend-api]
tags: [RAG, API-Authentication, Environment-Management, Python]
curated: 2026-06-16
curated_by: config-scout
---

# lanyuanzhe1/LLM — claude-md

**Why it's worth keeping:** The 'CRITICAL' warning regarding python -m pip to ensure environment consistency and the detailed HMAC authentication table are excellent transferable patterns for preventing common developer errors.

**Summary:** A highly specific technical guide for an iFlytek-based RAG pipeline involving specialized API authentication requirements.

**Source credibility:** Low-star repository, but high technical density suggests a real-world practical implementation.

**Recency:** Current; addresses modern platform-specific issues like dependency conflicts on Windows/Conda.

**Source:** [lanyuanzhe1/LLM/CLAUDE.md](https://github.com/lanyuanzhe1/LLM/blob/142ae574a2137c715169c692c97d32759f108cd2/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

Building a grain storage (粮食储藏) vertical-domain LLM RAG pipeline on iFlytek platform. Knowledge base: 17 documents (PDFs + DOCX, ~475K chars) covering pest control, low-temp storage, CO2 monitoring, smart granary management, and food security law.

## Environment

- Conda env: `ican` (Python 3.11.11) — always use this env
- **CRITICAL**: Use `python -m pip install <pkg>` — plain `pip` points to base conda (Python 3.13), which installs cp313-incompatible wheels
- GPU: RTX 4050 Laptop 8GB (CUDA available, not currently used by the pipeline)

## Key commands

```bash
python test_embedding_api.py      # Verify iFlytek Embedding API connectivity
python build_vector_store.py       # Full pipeline: read docs → chunk → vectorize → index → search
python search_kb.py                # Load existing vector store, interactive search only
```

## Architecture

```
knowledge/ (17 PDFs/DOCX)
    │  build_vector_store.py
    ▼
vector_store/
    vectors.npy          (1023 × 2560 float32)
    chunks_metadata.json (text + source per chunk)
    │  search_kb.py
    ▼
sklearn N
```

</details>
