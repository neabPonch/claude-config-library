---
name: clawic__skills__skill
source: https://github.com/clawic/skills/blob/ff40511e7588b7b91d4427b65931f420a7412bb0/skills/mongodb/SKILL.md
repo: clawic/skills
kind: skill
stars: 9
last_pushed: 2026-03-24T19:57:31Z
license: mit
score: 9
domains: [database, backend, devops]
tags: [mongodb, nosql, performance, architecture]
curated: 2026-06-16
curated_by: config-scout
---

# clawic/skills — skill

**Why it's worth keeping:** The file excels by documenting 'traps' (unbounded arrays, $lookup overhead) and actionable rules like the ESR indexing strategy rather than basic CRUD syntax.

**Summary:** A high-density expert guide for MongoDB that focuses on production-ready architecture, performance optimization, and common failure modes.

**Source credibility:** High-density content suggests a specialized developer source despite a modest star count.

**Recency:** Current; includes modern MongoDB features like version 5.0+ aggregation improvements and transaction considerations.

**Source:** [clawic/skills/skills/mongodb/SKILL.md](https://github.com/clawic/skills/blob/ff40511e7588b7b91d4427b65931f420a7412bb0/skills/mongodb/SKILL.md) · 9★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: MongoDB
slug: mongodb
version: 1.0.1
description: Design MongoDB schemas with proper embedding, indexing, aggregation, and production-ready patterns.
metadata: {"clawdbot":{"emoji":"🍃","requires":{"anyBins":["mongosh","mongo"]},"os":["linux","darwin","win32"]}}
---

## When to Use

User needs MongoDB expertise — from schema design to production optimization. Agent handles document modeling, indexing strategies, aggregation pipelines, consistency patterns, and scaling.

## Quick Reference

| Topic | File |
|-------|------|
| Schema design patterns | `schema.md` |
| Index strategies | `indexes.md` |
| Aggregation pipeline | `aggregation.md` |
| Production configuration | `production.md` |

## Schema Design Philosophy

- Embed when data is queried together and doesn't grow unboundedly
- Reference when data is large, accessed independently, or many-to-many
- Denormalize for read performance, accept update complexity—no JOINs means duplicate data
- Design for your queries, not for normalized elegance

## Document Size Traps

- 16MB max per document—plan for this from day one; use GridFS for large files
- Arrays that grow infinitely = disaster—use bucketing pattern instead
- BS
```

</details>
