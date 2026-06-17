---
name: scaleapi__scale-agentex
source: https://github.com/scaleapi/scale-agentex/blob/4b03f3abae83d2b5cb49ead3b317e15bfa986baf/CLAUDE.md
repo: scaleapi/scale-agentex
kind: claude-md
stars: 445
last_pushed: 2026-06-16T03:32:16Z
license: apache-2.0
score: 9
domains: [backend-api, agents-ai, security]
tags: [security-guardrails, command-reference, architectural-context]
curated: 2026-06-16
curated_by: config-scout
---

# scaleapi/scale-agentex — claude-md

**Why it's worth keeping:** The 'Public Repository' section provides essential negative constraints to prevent data leaks, while the structured 'Common Development Commands' allow an agent to execute tasks autonomously without guessing. The DDD architecture breakdown ensures the AI places new code in the correct layer.

**Summary:** A comprehensive guide that includes critical security redaction rules, extensive command glossaries for multiple environments, and architectural mental models.

**Source credibility:** High-quality industry repository from Scale AI with high star count and active maintenance.

**Recency:** Very current, utilizing modern toolchains like uv, Python 3.12, and Next.js.

**Source:** [scaleapi/scale-agentex/CLAUDE.md](https://github.com/scaleapi/scale-agentex/blob/4b03f3abae83d2b5cb49ead3b317e15bfa986baf/CLAUDE.md) · 445★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Public Repository

**This repository is public.** Everything that lands here — source code, comments, commit messages, file headers, runbooks, PR descriptions — is world-readable and indexed by search engines.

When making changes (especially commits, PR descriptions, and any operational docs), keep all of the following **out** of anything that gets pushed:

- Customer or account names (real or codename), and any identifying details about specific deployments, traffic patterns, or incidents tied to a customer.
- Internal Slack channels, threads, or permalinks (e.g. `scaleapi.slack.com/...`, `#some-internal-channel`).
- Internal ticket IDs and tracker URLs (Linear, Jira, etc.).
- Names or handles of individual employees, including in attribution like "per Alice's notes" or `Co-Authored-By` lines pointing at internal emails.
- Internal infrastructure references that aren't already documented publicly (internal hostnames, internal feature-flag system names, internal repo paths outside this one, etc.).
- Anything you wouldn't want a competitor or a journalist to read.
```

</details>
