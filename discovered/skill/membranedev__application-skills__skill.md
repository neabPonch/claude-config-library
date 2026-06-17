---
name: membranedev__application-skills__skill
source: https://github.com/membranedev/application-skills/blob/f484c8265e70ec910a57342389cca5c5de7d8167/skills/snowflake/SKILL.md
repo: membranedev/application-skills
kind: skill
stars: 224
last_pushed: 2026-04-28T08:45:44Z
license: unknown
score: 8
domains: [data-engineering, cli-tools, integration-patterns]
tags: [snowflake, membrane, auth-lifecycle, state-management]
curated: 2026-06-16
curated_by: config-scout
---

# membranedev/application-skills — skill

**Why it's worth keeping:** The state-polling logic (handling BUILDING/READY/CLIENT_ACTION_REQUIRED) and intent-based action discovery are highly transferable patterns for complex tool integration.

**Summary:** Provides a structured workflow for an agent to manage Snowflake connections and execute actions via the Membrane CLI.

**Source credibility:** Moderate; 224 stars indicates a legitimate, used utility by the developer community.

**Recency:** Current; it includes modern agent-specific instructions and follows contemporary CLI interaction patterns.

**Source:** [membranedev/application-skills/skills/snowflake/SKILL.md](https://github.com/membranedev/application-skills/blob/f484c8265e70ec910a57342389cca5c5de7d8167/skills/snowflake/SKILL.md) · 224★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: snowflake
description: |
  Snowflake integration. Manage data, records, and automate workflows. Use when the user wants to interact with Snowflake data.
compatibility: Requires network access and a valid Membrane account (Free tier supported).
license: MIT
homepage: https://getmembrane.com
repository: https://github.com/membranedev/application-skills
metadata:
  author: membrane
  version: "1.0"
  categories: ""
---

# Snowflake

Snowflake is a cloud-based data warehousing platform. It's used by data engineers, analysts, and scientists to store, process, and analyze large volumes of data. Think of it as a database built for the cloud.

Official docs: https://docs.snowflake.com/en/

## Snowflake Overview

- **Warehouse**
- **Database**
  - **Schema**
    - **Table**
- **Query**
  - Execute Query
  - Get Query Status
  - Get Query Result

## Working with Snowflake

This skill uses the Membrane CLI to interact with Snowflake. Membrane handles authentication and credentials refresh automatically — so you can focus on the integration logic rather than auth plumbing.

### Install the CLI

Install the Membrane CLI so you can run `membrane` from the terminal:

```bash
npm install
```

</details>
