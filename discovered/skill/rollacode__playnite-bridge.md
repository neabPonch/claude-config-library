---
name: rollacode__playnite-bridge
source: https://github.com/rollacode/playnite-bridge/blob/15bd0f8ddd220de0dca8b7a3076f597d69149b6b/skill.md
repo: rollacode/playnite-bridge
kind: skill
stars: 8
last_pushed: 2026-04-06T16:55:13Z
license: mit
score: 9
domains: [api-integration, local-automation, gaming]
tags: [rest-api, tool-definition, agent-skills]
curated: 2026-06-14
curated_by: config-scout
---

# rollacode/playnite-bridge — skill

**Why it's worth keeping:** It provides highly structured endpoint documentation with clear JSON schema examples and demonstrates the 'eval' pattern for high-agency tasks. The inclusion of specific query parameter types and complex 'groupBy' logic is an excellent template for tool-use files.

**Summary:** A comprehensive API specification that allows an AI agent to manage a local game library through RESTful commands and arbitrary C# execution.

**Source credibility:** Niche tool (8 stars) with recent maintenance activity.

**Recency:** Current; follows modern agentic documentation standards including placeholder patterns for secrets.

**Source:** [rollacode/playnite-bridge/skill.md](https://github.com/rollacode/playnite-bridge/blob/15bd0f8ddd220de0dca8b7a3076f597d69149b6b/skill.md) · 8★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Playnite Bridge — AI Skill

You have access to a Playnite game library manager running on the user's local machine.
Use HTTP requests (curl, fetch, etc.) to interact with it.

> **This file contains a personal API token. Do not share publicly.**

## Connection

- **Base URL:** `http://%%HOST%%:%%PORT%%`
- **Auth header:** `Authorization: Bearer %%TOKEN%%`
- **Format:** JSON (UTF-8)

## Endpoints

### Games

| Method | Path | Description |
|--------|------|-------------|
| GET | `/api/games` | List/search games (paginated) |
| GET | `/api/games/{id}` | Full game details |
| PUT | `/api/games/{id}` | Update game fields |
| DELETE | `/api/games/{id}` | Delete game from library |
| POST | `/api/games/{id}/launch` | Launch game |
| POST | `/api/games/{id}/install` | Start game installation |
| POST | `/api/games/{id}/uninstall` | Uninstall game |
| POST | `/api/games/{id}/fetch-art` | Fetch missing artwork |
| PUT | `/api/games/{id}/categories` | Set categories (replace) |
| POST | `/api/games/{id}/categories` | Add categories (append) |
| PUT | `/api/games/{id}/tags` | Set tags (replace) |
| POST | `/api/games/{id}/tags` | Add tags (append) |
| PUT | `/api/games/{id}/features` | Set
```

</details>
