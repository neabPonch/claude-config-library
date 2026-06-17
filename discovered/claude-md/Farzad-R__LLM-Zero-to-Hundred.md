---
name: Farzad-R__LLM-Zero-to-Hundred
source: https://github.com/Farzad-R/LLM-Zero-to-Hundred/blob/2bfd3a1d239f37b6906de06c9a6e5ad5a2d909c1/CLAUDE.md
repo: Farzad-R/LLM-Zero-to-Hundred
kind: claude-md
stars: 552
last_pushed: 2026-04-29T19:52:03Z
license: unknown
score: 7
domains: [agents-ai, machine-learning]
tags: [mono-repo, safety-guardrails, git-workflow]
curated: 2026-06-15
curated_by: config-scout
---

# Farzad-R/LLM-Zero-to-Hundred — claude-md

**Why it's worth keeping:** It effectively communicates how to navigate directory boundaries in a multi-project repo and provides essential safety guardrails to prevent accidental commits to the master branch.

**Summary:** Provides navigation guidance for a complex mono-repo containing multiple independent AI sub-projects and establishes strict Git workflow rules.

**Source credibility:** Strong; repository has significant stars (552) and recent maintenance activity.

**Recency:** 

**Source:** [Farzad-R/LLM-Zero-to-Hundred/CLAUDE.md](https://github.com/Farzad-R/LLM-Zero-to-Hundred/blob/2bfd3a1d239f37b6906de06c9a6e5ad5a2d909c1/CLAUDE.md) · 552★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a mono-repo of 9 independent LLM/RAG sub-projects and tutorials:

- `RAG-GPT` — document chat with ChromaDB + Gradio
- `WebGPT` — web-search-augmented chatbot with Streamlit
- `WebRAGQuery` — combines WebGPT and RAG-GPT with Chainlit
- `Hidden-Technical-Debt-Behind-AI-Agents` — LangGraph agentic chatbot with PostgreSQL + Docker
- `HUMAIN-advanced-multimodal-chatbot` — multimodal RAG (text, image, voice)
- `LLM-Fine-Tuning` — full fine-tuning pipeline with Chainlit UI
- `RAGMaster-LlamaIndex-vs-Langchain` — RAG technique comparison
- `Open-Source-RAG-GEMMA` — fully open-source RAG with Gemma + BAAI embeddings
- `tutorials/` — standalone notebooks and scripts (function calling, vectorization)

Each sub-project is fully self-contained with its own `requirements.txt`, `.env`, and — where present — its own `CLAUDE.md` with project-specific run commands and architecture details. The active conda environment is `refactor` (Python 3.11).

## Repo-Wide Conventions

**Commits** follow Conventional Commits:
- `feat:` new feature
- `fix:` bug fix
```

</details>
