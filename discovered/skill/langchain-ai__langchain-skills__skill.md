---
name: langchain-ai__langchain-skills__skill
source: https://github.com/langchain-ai/langchain-skills/blob/c88193a48f387560697e1152e32dc5fd239c83e4/config/skills/ecosystem-primer/SKILL.md
repo: langchain-ai/langchain-skills
kind: skill
stars: 795
last_pushed: 2026-06-08T14:16:24Z
license: unknown
score: 9
domains: [agents-ai, orchestration, frameworks]
tags: [langchain, primer, decision-logic, documentation-strategy]
curated: 2026-06-15
curated_by: config-scout
---

# langchain-ai/langchain-skills — skill

**Why it's worth keeping:** Uses a <decision-table> for deterministic tool selection and provides a robust documentation-retrieval strategy using llms.txt to minimize hallucinations in evolving libraries.

**Summary:** A high-level decision framework that directs an agent toward the correct tool (LangChain, LangGraph, or Deep Agents) based on task complexity.

**Source credibility:** High; official documentation/skills from the LangChain organization.

**Recency:** Extremely current, with activity within the last month.

**Source:** [langchain-ai/langchain-skills/config/skills/ecosystem-primer/SKILL.md](https://github.com/langchain-ai/langchain-skills/blob/c88193a48f387560697e1152e32dc5fd239c83e4/config/skills/ecosystem-primer/SKILL.md) · 795★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: ecosystem-primer
description: "INVOKE FIRST for any LangChain / LangGraph / Deep Agents agent building project before consulting other skills or writing any agent code. Required starting point for up to date info on framework selection (LangChain vs LangGraph vs Deep Agents vs hybrid composition), agent patterns, install, environment setup, and which skill to load next."
---

<overview>
LangChain Inc. maintains three layered open-source tools for building agents, plus LangSmith for observability. The stack, top-down:

- **Deep Agents** (top layer, *harness*) — batteries-included toolkit built on LangChain + LangGraph. Ships with planning, file management, subagent spawning, and memory out of the box.
- **LangGraph** (middle layer, *runtime*) — low-level orchestration for durable execution, custom control flow, and stateful workflows. LangChain agents run on top of LangGraph.
- **LangChain** (bottom layer, *framework*) — abstractions for models, tools, and the agent loop. Provider-agnostic, easiest to start with.
- **LangSmith** (cross-cutting) — observability and evaluation platform. Framework-agnostic; always recommended alongside any of the above.

Higher layers depend
```

</details>
