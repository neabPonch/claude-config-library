---
name: ECNU-ICALK__AutoSkill__skill
source: https://github.com/ECNU-ICALK/AutoSkill/blob/94c47ca488d4ba4117d20272e66d49b9877e68cf/SkillBank/ConvSkill/english_gpt4_8/generic-data-porting-server-architecture/SKILL.md
repo: ECNU-ICALK/AutoSkill
kind: skill
stars: 480
last_pushed: 2026-05-10T07:40:22Z
license: unknown
score: 7
domains: [backend-api, data-engineering]
tags: [etl, nodejs, architecture, mongodb]
curated: 2026-06-17
curated_by: config-scout
---

# ECNU-ICALK/AutoSkill — skill

**Why it's worth keeping:** It includes rigorous requirements for idempotency, specific data transformation rules (date normalization), and a highly structured directory layout perfect for automated scaffolding.

**Summary:** A detailed architectural blueprint for building a Node.js ETL (Extract, Transform, Load) pipeline that ingests files and forwards them to external APIs.

**Source credibility:** Moderate; the source is an academic repository with significant social proof via star count.

**Recency:** Current; utilizes modern Node.js/Express patterns and standard software engineering practices.

**Source:** [ECNU-ICALK/AutoSkill/SkillBank/ConvSkill/english_gpt4_8/generic-data-porting-server-architecture/SKILL.md](https://github.com/ECNU-ICALK/AutoSkill/blob/94c47ca488d4ba4117d20272e66d49b9877e68cf/SkillBank/ConvSkill/english_gpt4_8/generic-data-porting-server-architecture/SKILL.md) · 480★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
id: "cabe83d1-cfd1-46e1-96cb-d9de06744cd8"
name: "Generic Data Porting Server Architecture"
description: "Design a modular, scalable Node.js server architecture for ingesting Excel/CSV data, processing it with transaction-specific logic, storing it in MongoDB, and forwarding it to external APIs while ensuring idempotency and tracking processing time."
version: "0.1.0"
tags:
  - "nodejs"
  - "data-porting"
  - "architecture"
  - "mongodb"
  - "express"
triggers:
  - "create a generic data porting server"
  - "design architecture for excel csv to mongodb"
  - "node js data migration tool"
  - "transaction processing server with api forwarding"
  - "modular folder structure for data porting"
---

# Generic Data Porting Server Architecture

Design a modular, scalable Node.js server architecture for ingesting Excel/CSV data, processing it with transaction-specific logic, storing it in MongoDB, and forwarding it to external APIs while ensuring idempotency and tracking processing time.

## Prompt

# Role & Objective
Act as a Node.js Architect and Backend Developer. Design and implement a generic, modular, and scalable data porting server. The server must read data from Excel or CSV fi
```

</details>
