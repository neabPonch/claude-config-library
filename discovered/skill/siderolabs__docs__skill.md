---
name: siderolabs__docs__skill
source: https://github.com/siderolabs/docs/blob/bf1911323f93d1f98bf06f1891a213dc4efe3d03/public/skill.md
repo: siderolabs/docs
kind: skill
stars: 10
last_pushed: 2026-06-12T19:39:28Z
license: unknown
score: 9
domains: [devops, infrastructure-as-code, cli-tools]
tags: [talos, kubernetes, linux, siderolabs]
curated: 2026-06-15
curated_by: config-scout
---

# siderolabs/docs — skill

**Why it's worth keeping:** The 'Common gotchas' section is an excellent template for providing negative constraints to prevent LLM hallucinations (e.g., forbidding SSH/apt in a system that doesn't support them). It also includes clear, prescriptive command sequences and integration lists.

**Summary:** Provides specialized instructions for managing Talos Linux and Omni via API-driven workflows rather than traditional shell methods.

**Source credibility:** High; authored directly by the SideroLabs team.

**Recency:** Current; follows modern agentic prompting patterns with clear 'allowed behavior' boundaries.

**Source:** [siderolabs/docs/public/skill.md](https://github.com/siderolabs/docs/blob/bf1911323f93d1f98bf06f1891a213dc4efe3d03/public/skill.md) · 10★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: siderolabs
description: Deploy and operate Kubernetes clusters using Talos Linux and Omni. Use when generating/applying Talos machine configuration, managing cluster lifecycle in Omni, and troubleshooting common Talos/Omni workflows.
license: Apache-2.0
compatibility: Requires talosctl and/or omnictl. Talos is API-driven and does not support SSH.
metadata:
  author: siderolabs
  version: "1.0"
  mintlify-proj: siderolabs
---

# SideroLabs best practices

**Always consult the [Talos](https://docs.siderolabs.com/talos/v1.12/overview/what-is-talos) and [Omni](https://docs.siderolabs.com/omni/getting-started/getting-started) docs for configuration, latest features and best practices**

If you are not already connected to the SideroLabs MCP server, [https://docs.siderolabs.com/mcp](https://docs.siderolabs.com/mcp), add it so that you can search more efficiently.

Agents can use SideroLabs products to deploy, configure, and manage Kubernetes clusters at scale.

The SideroLabs created and currently manages two products:

- **Talos Linux**: Talos Linux is an API-Managed, secure, immutable, and minimal operating system for Kubernetes.
- **Talos Omni**: Omni is a Kubernetes managem
```

</details>
