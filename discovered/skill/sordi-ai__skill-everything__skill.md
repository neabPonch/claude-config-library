---
name: sordi-ai__skill-everything__skill
source: https://github.com/sordi-ai/skill-everything/blob/4e7dae3ff0c77e36538af2b1296904456919e73a/skills/langchain/SKILL.md
repo: sordi-ai/skill-everything
kind: skill
stars: 14
last_pushed: 2026-05-15T14:31:37Z
license: mit
score: 9
domains: [agents-ai, backend-api]
tags: [langchain, lcel, llm-orchestration, best-practices]
curated: 2026-06-16
curated_by: config-scout
---

# sordi-ai/skill-everything — skill

**Why it's worth keeping:** Mandates LCEL over legacy chains, enforces reliability via retry/timeout logic, and ensures observability through explicit tracing and typed output parsing.

**Summary:** Provides highly specific, opinionated rules for LangChain development to prevent the use of deprecated legacy classes and unobservable pipelines.

**Source credibility:** Niche repository with specialized intent; high quality of specific technical instructions despite modest star count.

**Recency:** Very current, focusing on modern patterns like LCEL, tool-calling agents, and recent LangChain structural changes.

**Source:** [sordi-ai/skill-everything/skills/langchain/SKILL.md](https://github.com/sordi-ai/skill-everything/blob/4e7dae3ff0c77e36538af2b1296904456919e73a/skills/langchain/SKILL.md) · 14★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: langchain
description: Apply when building LangChain pipelines, LCEL chains, agents, or retrieval-augmented generation systems.
license: MIT
version: 1.0.0
tokens_target: 2200
triggers:
  - langchain
  - lcel chain
  - agent framework
loads_after: [python]
supersedes: []
---

# Sub-Skill: LangChain / Agent Framework Conventions

**Purpose:** Prevent common LangChain mistakes — deprecated chain classes, missing retry/timeout guards, unsafe prompt handling, and unobservable pipelines.

---

## Rules

### Chain Construction

1. **Use LCEL pipe syntax.** Always use the LCEL pipe operator (`|`) to compose runnables instead of deprecated constructor-based chain classes (`LLMChain`, `SequentialChain`, `TransformChain`). Reference: ERR-2026-026
2. **Avoid legacy chain imports.** Never import from `langchain.chains.llm` or `langchain.chains.sequential`; use `langchain_core.runnables` and `langchain_core.prompts` instead.
3. **Prefer RunnablePassthrough for identity steps.** Use `RunnablePassthrough` to thread context through a chain without mutation rather than writing a lambda that returns its input unchanged.
4. **Use RunnableParallel for fan-out.** Prefer `RunnableParallel` ove
```

</details>
