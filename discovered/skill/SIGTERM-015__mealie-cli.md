---
name: SIGTERM-015__mealie-cli
source: https://github.com/SIGTERM-015/mealie-cli/blob/a4cbbc73ec4fe2c3776cc0c9b39ff0125d77272d/Skill.md
repo: SIGTERM-015/mealie-cli
kind: skill
stars: 0
last_pushed: 2026-02-25T00:05:55Z
license: unknown
score: 9
domains: [cli-tools, agents-ai, content-management]
tags: [recipe-management, json-schema, workflow-automation]
curated: 2026-06-14
curated_by: config-scout
---

# SIGTERM-015/mealie-cli — skill

**Why it's worth keeping:** It demonstrates the 'Plan -> Generate Schema -> Execute' workflow and includes specific domain-knowledge quirks (like mapping cook time to performTime) that prevent tool failure.

**Summary:** Provides detailed instructions for an agent to manage a Mealie recipe instance via CLI, focusing on converting unstructured recipes into highly structured JSON files.

**Source credibility:** Low visibility/stars; appears to be a specialized personal or niche utility.

**Recency:** Highly relevant for current agentic workflows involving CLI tools and structured data generation.

**Source:** [SIGTERM-015/mealie-cli/Skill.md](https://github.com/SIGTERM-015/mealie-cli/blob/a4cbbc73ec4fe2c3776cc0c9b39ff0125d77272d/Skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Mealie CLI Skill for AI Agents

Welcome, Agent. This document provides instructions on how to use the `mealie-cli` to interact with a user's Mealie instance.

## 1. Environment Requirements
The CLI is pre-configured to use environment variables for authentication. You do not need to pass tokens manually.
Make sure the following environment variables are set before invoking the tool (or instruct the user to set them):
- `MEALIE_URL`: The Mealie instance URL (e.g. `http://localhost:9000`)
- `MEALIE_API_KEY`: The API Token for authentication.

## 2. General Principles
- **Output:** All commands output strict JSON. Always parse the `stdout` as JSON. 
  - Success: `{"status": "success", "data": { ... }}`
  - Error: `{"status": "error", "message": "...", "details": { ... }}`
- **Idempotency:** When dealing with tags, categories, or tools, use the `ensure` commands. They will safely create the item if it doesn't exist or return its existing ID.

## 3. Creating Recipes
The most powerful feature of this CLI is creating recipes from an unstructured source (like a web page or text) using a simplified Agent JSON Schema. 

When a user asks you to import or create a recipe, follow these steps:
```

</details>
