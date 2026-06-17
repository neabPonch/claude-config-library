---
name: cch0__agentic-ai-localstack__adding-a-skill
source: https://github.com/cch0/agentic-ai-localstack/blob/5f17f43678cbc7bc77633cdaba188e578ca47106/docs/adding-a-skill.md
repo: cch0/agentic-ai-localstack
kind: skill
stars: 0
last_pushed: 2026-04-28T00:45:06Z
license: mit
score: 8
domains: [agents-ai, devops, backend-api]
tags: [skill-protocol, containerization, agentic-architecture]
curated: 2026-06-16
curated_by: config-scout
---

# cch0/agentic-ai-localstack — skill

**Why it's worth keeping:** The architecture decouples capability definition from execution logic, allowing tools to be language-agnostic and isolated in Docker. The use of AGENT.md for 'identity layer' injection provides a robust way to enforce hard constraints at the system level.

**Summary:** Defines a standardized, containerized protocol for building modular agent skills via dual HTTP endpoints (/schema and /execute). It automates tool discovery and persona injection through structured metadata files.

**Source credibility:** Low star count suggests a niche or new project, but high technical specificity indicates a functional framework.

**Recency:** Current; aligns with modern tool-calling standards and OpenAI/LiteLLM schema formats.

**Source:** [cch0/agentic-ai-localstack/docs/adding-a-skill.md](https://github.com/cch0/agentic-ai-localstack/blob/5f17f43678cbc7bc77633cdaba188e578ca47106/docs/adding-a-skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Adding a New Skill

The platform discovers skills automatically at startup. Adding a skill means creating a directory under `skills/`, building a Docker image that implements the skill contract, and restarting the server. No core code changes required.

---

## The contract

Every skill exposes two HTTP endpoints:

```
GET  /schema   → { "system_prompt": "...", "tools": [...] }
POST /execute  → { "tool": "tool_name", "params": {...} } → { "result": ... }
```

`/schema` is called once at startup. The platform reads the tool definitions and merges them with all other loaded skills — the LLM sees the full merged list every turn. `/execute` is called each time the LLM decides to use one of your tools.

The skill can be written in any language that can run an HTTP server.

---

## Directory structure

```
skills/
  your_skill/
    SKILL.md      ← metadata the platform reads + human-readable docs
    AGENT.md      ← optional: skill identity and hard constraints injected at L0
    .env          ← secrets injected into the container at start
    Dockerfile
    main.py       ← or whatever your skill is written in
```

### SKILL.md

Two fields are required:

```markdown
---
name: your_skil
```

</details>
