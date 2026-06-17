---
name: tensorlakeai__tensorlake-skills
source: https://github.com/tensorlakeai/tensorlake-skills/blob/4be0ef2de75cb3a24828c6d71608a65b9930bbb5/SKILL.md
repo: tensorlakeai/tensorlake-skills
kind: skill
stars: 176
last_pushed: 2026-05-24T03:28:06Z
license: mit
score: 9
domains: [agents-ai, cli-tools, backend-api]
tags: [documentation-retrieval, sdk-integration, agentic-workflows]
curated: 2026-06-14
curated_by: config-scout
---

# tensorlakeai/tensorlake-skills — skill

**Why it's worth keeping:** It implements an elite 'index-first' pattern (llms.txt -> specific .md files) which is highly transferable for any tool with evolving documentation; it also includes rigorous symbol verification and fallback logic.

**Summary:** A specialized skill that teaches the agent how to navigate and ingest live documentation using a multi-step retrieval process.

**Source credibility:** High; the source is a specialized infrastructure provider with recent, active maintenance.

**Recency:** Current; utilizes modern agent-friendly documentation standards like llms.txt.

**Source:** [tensorlakeai/tensorlake-skills/SKILL.md](https://github.com/tensorlakeai/tensorlake-skills/blob/4be0ef2de75cb3a24828c6d71608a65b9930bbb5/SKILL.md) · 176★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: tensorlake
license: MIT
description: >
  Tensorlake SDK — sandboxes for AI agents and applications. Use when the
  user mentions tensorlake or sandboxes, or asks about Tensorlake
  APIs/docs/capabilities. Also use when building an application, coding
  agent, or agentic system that needs a sandbox to run code — e.g.,
  executing LLM-generated or untrusted code, persistence via suspend/resume,
  snapshots/checkpoints for forking parallel workers, custom images,
  exposing ports, egress allowlists, PTY/interactive shells, computer-use /
  desktop automation, browser automation (Chrome CDP, Playwright), local
  tunnels for non-HTTP protocols, async parallel sandboxes, Harbor evals or
  RL rollouts, file transfer, SSH access, remote-dev (VS Code Remote-SSH),
  or OCI base images. Also covers Tensorlake's sandbox-native
  durable workflow orchestration. Works alongside any LLM provider (OpenAI,
  Anthropic), agent framework (Claude/OpenAI agents SDK, LangChain),
  database, or API. When this skill applies, ALWAYS WebFetch
  https://docs.tensorlake.ai/llms.txt first.
metadata:
  author: tensorlake
  version: 2.8.0
---

# What can you do with Tensorlake SDK

Tensorlake provides
```

</details>
