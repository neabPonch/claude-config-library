---
name: sam1730__caresync
source: https://github.com/sam1730/caresync/blob/610eafe9531d58c387a4ac55b3768ab8bbbf592d/CLAUDE.MD
repo: sam1730/caresync
kind: claude-md
stars: 0
last_pushed: 2026-03-27T15:48:54Z
license: mit
score: 9
domains: [backend-api, data-engineering]
tags: [monorepo, fhir, high-context]
curated: 2026-06-14
curated_by: config-scout
---

# sam1730/caresync — claude-md

**Why it's worth keeping:** It embeds concrete data mappings (LOINC codes) and exact configuration file contents to eliminate ambiguity during implementation.

**Summary:** A comprehensive technical specification that includes architecture rules, full type definitions, and explicit business mapping logic.

**Source credibility:** Low social proof (0 stars), but content is highly structured and professionally detailed.

**Recency:** Current; targets Node.js 22 and modern TypeScript patterns.

**Source:** [sam1730/caresync/CLAUDE.MD](https://github.com/sam1730/caresync/blob/610eafe9531d58c387a4ac55b3768ab8bbbf592d/CLAUDE.MD) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## Project Overview

CareSync is a headless TypeScript monorepo and open-source npm library for syncing wearable health data into Salesforce Health Cloud.

Core pipeline:

1. Pull health data from wearable devices via the Open Wearables API
2. Normalise raw data into a clean internal schema
3. Map the data to FHIR R4 `Observation` resources
4. Authenticate with Salesforce via OAuth 2.0
5. Upsert FHIR records into Salesforce Health Cloud

A local mock server is included so developers can test without a real Salesforce org.

## High-level rules

- This project is headless. Do not add a UI unless explicitly requested.
- Keep the library backend-friendly and reusable.
- Use TypeScript throughout.
- Use an npm workspaces monorepo layout.
- Target Node.js 22+ and npm 10+.
- Favor strict typing and clear interfaces.
- Keep modules small and testable.
- Keep transformation logic pure where possible.
- Isolate side effects to connectors, network clients, and server code.
- Do not hardcode secrets or credentials.

## Repository structure

Expected layout:

```text
caresync/
├── packages/
│   ├── core/
│   │   ├── src/
│   │   │   ├���─ normaliser.ts
│   │   │   ├── fhir-mapper.t
```

</details>
