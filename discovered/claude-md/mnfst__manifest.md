---
name: mnfst__manifest
source: https://github.com/mnfst/manifest/blob/57cce76c5e0ea072212580203d4d905b55a2204a/CLAUDE.md
repo: mnfst/manifest
kind: claude-md
stars: 6970
last_pushed: 2026-06-15T09:13:38Z
license: mit
score: 9
domains: [backend-api, ai-agents, dev-ops]
tags: [monorepo, typeorm, nestjs, database-isolation]
curated: 2026-06-15
curated_by: config-scout
---

# mnfst/manifest — claude-md

**Why it's worth keeping:** Includes copy-pasteable shell commands for database isolation to prevent state pollution and a comprehensive directory tree that maps file roles/purposes.

**Summary:** Provides high-fidelity architectural context including complex dev-environment setup and specific integration testing workflows.

**Source credibility:** High: 6.9k stars on GitHub with very recent maintenance activity.

**Recency:** Extremely current; uses modern tech stacks like NestJS 11 and Node 24.

**Source:** [mnfst/manifest/CLAUDE.md](https://github.com/mnfst/manifest/blob/57cce76c5e0ea072212580203d4d905b55a2204a/CLAUDE.md) · 6970★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Manifest Development Guidelines

Last updated: 2026-04-12

## What Manifest Is

Manifest is a smart model router for **AI agents**. It sits between an agent and its LLM providers, scores each request, and routes it to the cheapest model that can handle it. The dashboard tracks costs, tokens, and messages across any agent that speaks OpenAI-compatible HTTP.

**Supported agents** (configured in `packages/shared/src/agent-type.ts`): OpenClaw, Hermes, OpenAI SDK, Vercel AI SDK, LangChain, cURL, and a generic `other` slot. OpenClaw remains the deepest integration, but no new code or copy should frame Manifest as OpenClaw-only. When adding examples, prefer "AI agent" as the noun and pick OpenClaw as the worked example rather than the sole target. Manifest is consumed as a generic OpenAI-compatible HTTP endpoint — there are no first-party OpenClaw plugins in this repo anymore.

Wingman — the gateway tester for sending requests against a Manifest backend while impersonating any of the supported agents (useful for routing/header-classifier reproductions) — lives in its own repo at [`mnfst/wingman`](https://github.com/mnfst/wingman) and is hosted at [`wingman.manifest.build`](https://wingm
```

</details>
