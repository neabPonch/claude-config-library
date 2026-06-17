---
name: AhirTech1__MarginFlow__claude
source: https://github.com/AhirTech1/MarginFlow/blob/9e6ce0da85ecafd96c9a28573e8c617a6c7637ef/agents/claude.md
repo: AhirTech1/MarginFlow
kind: claude-md
stars: 0
last_pushed: 2026-06-04T12:46:33Z
license: mit
score: 7
domains: [agents-ai, devops-automation]
tags: [constraints, sandboxing, scope-limitation, agentic-workflow]
curated: 2026-06-14
curated_by: config-scout
---

# AhirTech1/MarginFlow — claude-md

**Why it's worth keeping:** Uses high-signal negative constraints ('STRICTLY FORBIDDEN') and path whitelisting to prevent lateral movement into unrelated directories. Includes a mandatory pre-flight check against a PROJECT_TRACKER.md to ensure schema compliance.

**Summary:** Defines strict operational boundaries and scope-limiting constraints for an AI agent focused on a specific sub-module.

**Source credibility:** Low; single-repo source with no social proof or historical maintenance indicated.

**Recency:** Current; utilizes advanced agentic constraint patterns seen in modern LLM orchestration.

**Source:** [AhirTech1/MarginFlow/agents/claude.md](https://github.com/AhirTech1/MarginFlow/blob/9e6ce0da85ecafd96c9a28573e8c617a6c7637ef/agents/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Agents AI Session Constraints

## SYSTEM RULE

You are the **AI Orchestration Assistant**. You are **STRICTLY FORBIDDEN** from reading or modifying any files outside the `agents/` directory. Focus only on Gemini API prompts, ChromaDB RAG logic, and OpenClaw routing.

## BOUNDARIES

- **Allowed paths**: `agents/`, `agents/router.js`, `agents/rag_worker.js`, `agents/synthesizer.js`
- **Forbidden paths**: `frontend/`, `backend/`, `README.md` (root), `.gitignore` (root)
- **Allowed operations**: Creating, updating, and deleting files within `agents/`
- **Forbidden operations**: Any `npm install` outside `agents/`, editing root-level files, touching `frontend/` or `backend/` directories

## FOCUS AREAS

1. Gemini API prompt engineering and safety settings
2. ChromaDB collection management and vector search logic
3. Agent routing and task decomposition in `router.js`
4. RAG pipeline implementation in `rag_worker.js`
5. Output synthesis and error aggregation in `synthesizer.js`

## GLOBAL RULE

Before executing npm installs, ensure you are inside your designated directory. Do not touch the root package.json. Commit only files within your domain to prevent git merge conflicts.

## PROJEC
```

</details>
