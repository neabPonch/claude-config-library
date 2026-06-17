---
name: AudiusProject__apps__skill
source: https://github.com/AudiusProject/apps/blob/5ec7686838732df9f165f3f1523a500430a1fe68/packages/web/public/skill.md
repo: AudiusProject/apps
kind: skill
stars: 611
last_pushed: 2026-06-11T21:54:41Z
license: apache-2.0
score: 9
domains: [backend-api, agents-ai, web-frontend]
tags: [api-integration, openapi, sdk-context, image-handling]
curated: 2026-06-15
curated_by: config-scout
---

# AudiusProject/apps — skill

**Why it's worth keeping:** Includes machine-readable OpenAPI/Swagger URLs for automated contract ingestion and highly specific logic for handling image mirror retry patterns to prevent asset failures.

**Summary:** Provides specialized context for interacting with the Audius music platform via REST API and JS SDK.

**Source credibility:** High; sourced from an active, high-star open-source monorepo.

**Recency:** Modern; includes current standards like OpenAPI 3.0 and Vite/React workflows.

**Source:** [AudiusProject/apps/packages/web/public/skill.md](https://github.com/AudiusProject/apps/blob/5ec7686838732df9f165f3f1523a500430a1fe68/packages/web/public/skill.md) · 611★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: audius-api-sdk
version: 1.0
description: Build on Audius—REST API, OpenAPI/Swagger, JavaScript SDK, create-audius-app
homepage: https://audius.co
metadata:
  {
    'api': 'api.audius.co/v1',
    'swagger': 'api.audius.co/v1/swagger.yaml',
    'sdk': '@audius/sdk',
    'scaffold': 'create-audius-app'
  }
---

# Audius API and SDK Skill

This file provides agentic context for building on Audius with the REST API, OpenAPI/Swagger spec, JavaScript SDK, and create-audius-app. For high-level protocol and product context, read [agents.md](https://audius.co/agents.md) first.

**Recommendations, not rules.** Use maximal creativity—remix, extend, invent. Agentic apps use Audius as the open standard for music. This is your toolkit.

## Overview

Audius exposes a REST API and a JavaScript SDK for the same backend. Use the API directly for any language or custom integrations; use the SDK for TypeScript/JavaScript apps. Both require API credentials. The OpenAPI/Swagger spec is machine-readable—ingest it for codegen, tooling, or AI-assisted development. create-audius-app scaffolds a ready-to-run project. Pick what fits your vision and go beyond it.

## Quickstart

```sh
npx create-audiu
```

</details>
