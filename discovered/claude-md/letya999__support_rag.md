---
name: letya999__support_rag
source: https://github.com/letya999/support_rag/blob/68f69b44c8a4a3830d1b4dd677f4a28222e9d3ef/claude.md
repo: letya999/support_rag
kind: claude-md
stars: 1
last_pushed: 2026-01-16T19:03:04Z
license: mit
score: 9
domains: [agents-ai, backend-api, rag]
tags: [langgraph, fastapi, production-grade]
curated: 2026-06-15
curated_by: config-scout
---

# letya999/support_rag — claude-md

**Why it's worth keeping:** Includes explicit architectural flow diagrams, strict API response patterns (Envelope pattern), and critical developer rules regarding configuration management and service statelessness.

**Summary:** A highly detailed blueprint for a production-grade LangGraph RAG pipeline featuring complex node orchestration and specialized data staging logic.

**Source credibility:** Low star count but demonstrates high engineering maturity through sophisticated system design and constraint documentation.

**Recency:** Very current; utilizes modern frameworks like LangGraph 1.0+ and GPT-4o-mini.

**Source:** [letya999/support_rag/claude.md](https://github.com/letya999/support_rag/blob/68f69b44c8a4a3830d1b4dd677f4a28222e9d3ef/claude.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Support RAG - Production Q&A Pipeline

Production-grade Retrieval-Augmented Generation system for customer support. Answers ONLY from retrieved context with LangGraph 22-node pipeline, PostgreSQL+pgvector, Qdrant, Redis. Built with groundedness guarantees, multi-turn conversations, and Telegram integration.

**Core Principle:** Answer from context or escalate to humans. Never hallucinate.

## Tech Stack

**Framework:** LangGraph ≥1.0.5, LangChain ≥1.2.0, FastAPI ≥0.128.0  
**LLM:** OpenAI gpt-4o-mini, sentence-transformers embeddings  
**Storage:** PostgreSQL+pgvector (docs+metadata), Qdrant (vectors), Redis (cache+staging)  
**ML/NLP:** PyTorch, FastText, llm-guard, RAGAS, Langfuse  
**Docs:** PyPDF, python-docx, pandas (CSV/JSON/PDF/DOCX)

## Architecture

### LangGraph Pipeline (22 Nodes)
```
Input → InputGuardrails → CacheCheck → LanguageDetection → DialogAnalysis
 → QueryAggregation → QueryTranslation → EasyClassification → MetadataFiltering
 → HybridSearch → Reranking → MultiHopReasoning → Fusion → StateDecision
 → Routing → PromptSelection → Generation → OutputGuardrails → ArchiveSession → CacheStore
```

Each node has isolated `config.yaml` → auto-merged into `pipeline_co
```

</details>
