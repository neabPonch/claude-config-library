---
name: hoangsonww__EstateWise-Chapel-Hill-Chatbot
source: https://github.com/hoangsonww/EstateWise-Chapel-Hill-Chatbot/blob/92f7b6f9433af7fb3aecf2b2e3eb954ba51e5803/CLAUDE.md
repo: hoangsonww/EstateWise-Chapel-Hill-Chatbot
kind: claude-md
stars: 32
last_pushed: 2026-06-16T15:43:11Z
license: mit
score: 9
domains: [monorepo, agents-ai, fullstack]
tags: [skill-system, context-management, monorepo]
curated: 2026-06-16
curated_by: config-scout
---

# hoangsonww/EstateWise-Chapel-Hill-Chatbot — claude-md

**Why it's worth keeping:** It employs an advanced '/skill' system to offload deep documentation into on-demand files and provides high-signal 'Gotchas' that address specific architectural pitfalls.

**Summary:** A sophisticated monorepo guide that uses a tiered 'Skill' pattern to manage context window limits and project complexity.

**Source credibility:** High; features a complex, actively maintained agentic AI architecture.

**Recency:** 

**Source:** [hoangsonww/EstateWise-Chapel-Hill-Chatbot/CLAUDE.md](https://github.com/hoangsonww/EstateWise-Chapel-Hill-Chatbot/blob/92f7b6f9433af7fb3aecf2b2e3eb954ba51e5803/CLAUDE.md) · 32★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# EstateWise Claude Code Memory

This file is the always-on memory for Claude Code in this repository. Keep it lean. Put deep reference material and repeatable workflows in project skills under `.claude/skills/` so they load on demand instead of every session.

## Use The Right Skill

- `/estatewise-engineering` for most code changes anywhere in the monorepo.
- `/estatewise-review` for PR review, diff review, bug hunt, regression checks, or test-gap review.
- `/estatewise-contracts` when REST, tRPC, MCP, gRPC, A2A, or shared payloads might change.
- `/estatewise-ai-runtime` when work touches MCP, agentic-ai, web-grounding, token flows, or A2A.
- `/estatewise-local-stack` for local setup, run commands, service combinations, and environment debugging.
- `/estatewise-ops` for deployment-control, Docker, Kubernetes, Helm, Terraform, Jenkins, or cloud deployment assets.

## Always-On Rules

- Make surgical changes only. Do not refactor unrelated modules.
- Preserve existing contracts unless the task explicitly requests a breaking change.
- If you change a producer contract, update the consumer path in the same task.
- Run the smallest relevant validation for touched packages before hand
```

</details>
