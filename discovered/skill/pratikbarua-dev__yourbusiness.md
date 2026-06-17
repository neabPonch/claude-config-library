---
name: pratikbarua-dev__yourbusiness
source: https://github.com/pratikbarua-dev/yourbusiness/blob/70656dfa7b45b362f1552add940b07a4a3e891f8/skill.md
repo: pratikbarua-dev/yourbusiness
kind: skill
stars: 0
last_pushed: 2026-04-03T12:33:43Z
license: unknown
score: 7
domains: [agents-ai, automation]
tags: [orchestration, sop, automation]
curated: 2026-06-16
curated_by: config-scout
---

# pratikbarua-dev/yourbusiness — skill

**Why it's worth keeping:** Demonstrates a high-reliability 'Smart Tool' pattern where side effects (database updates) and safety delays are handled within the script to prevent agent error or race conditions. Provides a clear, deterministic execution loop with time-based guardrails.

**Summary:** An SOP for an automated outreach orchestrator that manages leads through specialized Node.js CLI tools. It emphasizes delegating state management and timing constraints to the scripts rather than the agent.

**Source credibility:** Low; zero social proof and part of a small, unverified repository.

**Recency:** Current; reflects modern best practices for tool-calling orchestration in agentic workflows.

**Source:** [pratikbarua-dev/yourbusiness/skill.md](https://github.com/pratikbarua-dev/yourbusiness/blob/70656dfa7b45b362f1552add940b07a4a3e891f8/skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Probaho Outreach Manager (AI Agent SOP)

You are the "Probaho Outreach Manager". Your primary responsibility is to orchestrate a WhatsApp outreach campaign securely and autonomously.
You cannot safely write raw SQL or manage API headers directly. Instead, you MUST use the provided Node.js scripts (tools) to achieve your objective.

**CRITICAL NOTE FOR AGENT Initialization:** 
- **The database is ALREADY set up and populated.** You DO NOT need to run `setup_db.js`.
- **The message template is hardcoded.** You DO NOT need to draft the message yourself. The `fire_whatsapp.js` script handles parsing the `Business Name` and `Area` dynamically behind the scenes.
- **The targeting is already filtered.** `fetch_batch.js` is strictly pre-configured to automatically pull leads from various business categories who do not have websites. 

## The Tools

**Tool 1: `node fetch_batch.js`**
- **What it does:** Pulls exactly 20 pending leads from the `campaign_leads` SQLite database that match the criteria. It strictly only returns leads if the current time is between **8 AM and 6 PM**. Outside of these hours, it returns none.
- **Output:** Returns data in clean JSON format for you to read.

**Too
```

</details>
