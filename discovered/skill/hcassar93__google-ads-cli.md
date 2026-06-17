---
name: hcassar93__google-ads-cli
source: https://github.com/hcassar93/google-ads-cli/blob/36961a5d5212b936597a36865f95c7f980ad5ba7/skill.md
repo: hcassar93/google-ads-cli
kind: skill
stars: 0
last_pushed: 2026-03-30T06:16:16Z
license: mit
score: 8
domains: [cli-tools, marketing-api, automation]
tags: [google-ads, runbooks, operational-guide]
curated: 2026-06-14
curated_by: config-scout
---

# hcassar93/google-ads-cli — skill

**Why it's worth keeping:** The use of 'high-confidence automation runbooks' and explicit mandates for `--json` output provides a perfect blueprint for turning standard CLI tools into reliable agent skills.

**Summary:** Provides structured operational intelligence for using the Google Ads CLI in agentic workflows, including setup, reporting, and error handling.

**Source credibility:** Low social proof (0 stars), but the document structure suggests a practical, high-quality tool implementation.

**Recency:** Current; follows modern patterns for agentic tool usage.

**Source:** [hcassar93/google-ads-cli/skill.md](https://github.com/hcassar93/google-ads-cli/blob/36961a5d5212b936597a36865f95c7f980ad5ba7/skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: google-ads-cli-skill
description: Comprehensive operational guide for agents using Google Ads CLI.
version: 1.0.0
tools:
  - google-ads-cli
---

# Google Ads CLI Skill (`google-ads-cli`)

This skill trains an agent to operate `google-ads-cli` reliably in automation and agentic pipelines.

## 1) Tool identity

- Package: `google-ads-cli`
- Binary: `google-ads-cli`
- Local dev entry: `npm run dev -- <command>`

## 2) Capabilities

The CLI supports:

- Setup and credential/profile management
- OAuth authentication
- Account listing
- Campaign and ad group inspection
- Keyword Planner idea generation
- Geo target location lookup
- GAQL query execution

## 3) Prerequisites and readiness checks

Preflight checks:

1. Node >= 18
2. Setup completed (`setup`)
3. Authenticated profile (`auth`)
4. Required account context exists (customer ID/login customer ID)

Readiness commands:

```bash
google-ads-cli --version
google-ads-cli --help
google-ads-cli config
google-ads-cli profiles --list
```

## 4) First-time workflow

### 4.1 Setup

```bash
google-ads-cli setup
```

Provide:

- OAuth client ID
- OAuth client secret
- Developer token
- Customer ID (no dashes)
- Optional login custom
```

</details>
