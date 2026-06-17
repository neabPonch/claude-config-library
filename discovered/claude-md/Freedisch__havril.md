---
name: Freedisch__havril
source: https://github.com/Freedisch/havril/blob/3a05f55fd14ab728a74eb814cd7f8ff52b5c74f0/Claude.md
repo: Freedisch/havril
kind: claude-md
stars: 4
last_pushed: 2026-05-29T07:27:59Z
license: mit
score: 9
domains: [backend-api, agents-ai, go]
tags: [architectural-blueprint, schema-driven, system-design]
curated: 2026-06-15
curated_by: config-scout
---

# Freedisch/havril — claude-md

**Why it's worth keeping:** It includes explicit SQL schemas with index definitions and Go interface signatures, which prevents an AI from hallucinating incorrect methods or database structures. The 'Architecture in One Paragraph' provides vital mental models of how data flows through the services.

**Summary:** This file serves as a high-density architectural blueprint that defines the entire system's data model, service interfaces, and project topology.

**Source credibility:** High; a well-structured, modern Go project with recent activity and clear architectural intent.

**Recency:** Very current; uses modern Go (1.22+) and relevant AI/MCP ecosystem patterns.

**Source:** [Freedisch/havril/Claude.md](https://github.com/Freedisch/havril/blob/3a05f55fd14ab728a74eb814cd7f8ff52b5c74f0/Claude.md) · 4★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Havril

— Claude Code Context

## What This Project Is

Havril
is a **model-agnostic memory service** written in Go. It gives AI models (Claude,
ChatGPT, Gemini, Mistral, etc.) the ability to remember users persistently across
conversations — regardless of which platform they use.

**Havril
is not a chat interface.** It is a pure backend memory layer. Users keep chatting
on Claude.ai, ChatGPT.com, Gemini, etc. exactly as they do today. Havril
plugs into those
platforms as a tool integration and works silently in the background.

**The intelligence lives inside Havril
, not the models.** Models are delivery pipes — they
submit raw conversations and receive distilled memories back. Havril
's Memory Engine decides
what is worth keeping, how important it is, and how to reconcile it with existing knowledge.

---

## Architecture in One Paragraph

Users sign up, get a Bearer token, and connect their AI platforms (Claude via MCP, ChatGPT
via Custom Action). When a model conversation ends, the model calls `POST /v1/memory/submit`
with the raw transcript. Havril
's Memory Engine processes it: extract facts with an internal
LLM → deduplicate against Qdrant → resolve contradictions → score
```

</details>
