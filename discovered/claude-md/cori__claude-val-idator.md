---
name: cori__claude-val-idator
source: https://github.com/cori/claude-val-idator/blob/31cd7ccff32fda7f599b256c0d5ecd1c6f0569e3/claude.md
repo: cori/claude-val-idator
kind: claude-md
stars: 0
last_pushed: 2026-06-08T15:02:09Z
license: unknown
score: 8
domains: [backend-api, serverless, deno]
tags: [val-town, tdd, deno]
curated: 2026-06-15
curated_by: config-scout
---

# cori/claude-val-idator — claude-md

**Why it's worth keeping:** Includes high-value code snippets for domain-specific SDKs (auth, storage) to prevent hallucination of standard Node.js patterns.

**Summary:** Provides deep technical context for the Val.town/Deno ecosystem and establishes a strict Red-Green-Refactor development workflow.

**Source credibility:** Low star count suggests it's an emerging or private template, but the technical density is high.

**Recency:** Current; aligned with modern Deno and Val.town standards.

**Source:** [cori/claude-val-idator/claude.md](https://github.com/cori/claude-val-idator/blob/31cd7ccff32fda7f599b256c0d5ecd1c6f0569e3/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Code Guide for Val.town Development

This repository is a template for building Val.town vals using Claude Code. This guide captures essential knowledge about working with Val.town and establishes development best practices.

We'll be working on the repo through GitHub issues; as soon as you've finished reading this file make sure you have the `gh` client installed and that you can access issues. You can install it with `apt-get install -y gh`.

## Collaboration

### Pull Requests & Commits

- Do not include session URLs, agent names, or tool identifiers in PR bodies, commit messages, or code comments — keep those to chat only
- PR descriptions: summary bullets + a test plan checklist is enough
- Always reference the closing issue with `Resolves #X` (or `Closes #X`) in the PR body so GitHub auto-closes it on merge

## Val.town Essentials

### What is Val.town?

Val.town is a serverless platform for running JavaScript/TypeScript code. Each "val" is a function that can be:
- HTTP endpoints (web servers, APIs, webhooks)
- Scheduled functions (cron jobs)
- Email handlers
- Background jobs

### Val.town Runtime Environment

- **Runtime**: Deno runtime with web-standard APIs
- *
```

</details>
