---
name: jamierpond__yapi__skill
source: https://github.com/jamierpond/yapi/blob/e191d6e9d7180b02d2b6caa10aaf231f8035753a/docs/topics/skill.md
repo: jamierpond/yapi
kind: skill
stars: 110
last_pushed: 2026-02-28T01:01:36Z
license: mit
score: 8
domains: [cli-tools, backend-api, testing]
tags: [api-client, yaml, test-automation, request-chaining]
curated: 2026-06-15
curated_by: config-scout
---

# jamierpond/yapi — skill

**Why it's worth keeping:** It provides clear, reproducible patterns for complex agentic tasks like authentication chaining via variable interpolation and automated response validation using JQ expressions.

**Summary:** A highly structured skill guide for yapi, a CLI tool designed for Git-friendly, YAML-based API orchestration and testing.

**Source credibility:** Strong; 110 stars indicates a vetted, useful developer utility.

**Recency:** Current; last updated 4 months ago.

**Source:** [jamierpond/yapi/docs/topics/skill.md](https://github.com/jamierpond/yapi/blob/e191d6e9d7180b02d2b6caa10aaf231f8035753a/docs/topics/skill.md) · 110★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# yapi — LLM Skill Guide

yapi is a CLI-first, git-friendly API client. You define requests in YAML files and run them from the terminal. No GUI, no accounts, no state — just files and a binary.

## When to Use yapi

- Send HTTP, gRPC, GraphQL, or TCP requests
- Chain multiple requests together (auth flow, then use the token)
- Assert on responses (status codes, body content via JQ)
- Run API test suites with `yapi test`
- Poll endpoints until a condition is met

## Core Concepts

**Every request file starts with `yapi: v1`.** This is required.

**File extension:** `.yapi.yml` (or `.yapi.yaml`). Test files use `.test.yapi.yml`.

**Project config:** `yapi.config.yml` at the project root defines environments and base URLs. yapi walks up the directory tree to find it.

**Variables:** Use `${VAR}` syntax. Resolved from: chain step outputs > environment vars > shell env > defaults. Default values: `${VAR:-fallback}`.

## Quick Reference

### Run a request file

```bash
yapi run request.yapi.yml
yapi run request.yapi.yml -e prod   # with environment
```

### Quick one-off request (no file needed)

```bash
yapi send https://api.example.com/users           # GET
yapi send https://api.examp
```

</details>
