---
name: apify__agent-skills__skill
source: https://github.com/apify/agent-skills/blob/18297b635a8e50a6bfa080662c0a0e3cc3abbb1a/skills/apify-sdk-integration/SKILL.md
repo: apify/agent-skills
kind: skill
stars: 2148
last_pushed: 2026-06-02T07:46:07Z
license: unknown
score: 9
domains: [backend-api, web-scraping, automation]
tags: [apify, sdk-integration, javascript, python]
curated: 2026-06-15
curated_by: config-scout
---

# apify/agent-skills — skill

**Why it's worth keeping:** Includes a 'Critical' section to prevent common package-name mistakes (apify vs apify-client) and provides clear distinctions between synchronous and asynchronous execution patterns.

**Summary:** Provides comprehensive implementation patterns for integrating Apify Actors into JS/TS and Python applications using the client SDK or REST API.

**Source credibility:** High; Apify is an industry-standard web scraping platform with highly active development.

**Recency:** 

**Source:** [apify/agent-skills/skills/apify-sdk-integration/SKILL.md](https://github.com/apify/agent-skills/blob/18297b635a8e50a6bfa080662c0a0e3cc3abbb1a/skills/apify-sdk-integration/SKILL.md) · 2148★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: apify-sdk-integration
description: Integrate Apify into an existing JavaScript/TypeScript or Python application using the apify-client package. Use when adding web scraping, automation, or data extraction capabilities to an existing app via the Apify API.
---

# Apify SDK Integration

Add Apify Actor execution to an existing application. This skill covers the `apify-client` package for JS/TS and Python, plus the REST API for other languages.

## When to Use This Skill

- Adding web scraping or automation to an existing app
- Calling Apify Actors programmatically from application code
- Building a product that uses Apify as a backend service
- Integrating Actor results into a data pipeline

## Critical: Package Naming

> **`apify-client`** is the API client for **calling** Actors from your app.
> **`apify`** is the SDK for **building** Actors (wrong package for this use case).
>
> Always install `apify-client`. Never install `apify` for integration work.

## Prerequisites

The user needs an `APIFY_TOKEN`. Direct them to **Console > Settings > Integrations** at https://console.apify.com/settings/integrations to create one. If they don't have an account: https://console.apif
```

</details>
