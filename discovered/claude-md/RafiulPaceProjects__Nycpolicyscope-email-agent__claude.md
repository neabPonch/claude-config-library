---
name: RafiulPaceProjects__Nycpolicyscope-email-agent__claude
source: https://github.com/RafiulPaceProjects/Nycpolicyscope-email-agent/blob/6d0ff520520e2aa19557acc5ed2ad7c9dcc22f42/nanoclaw/groups/n8n-expert/CLAUDE.md
repo: RafiulPaceProjects/Nycpolicyscope-email-agent
kind: claude-md
stars: 0
last_pushed: 2026-03-19T16:06:56Z
license: mit
score: 9
domains: [automation, devops, ai-agents]
tags: [troubleshooting-patterns, technical-reference, workflow-automation]
curated: 2026-06-16
curated_by: config-scout
---

# RafiulPaceProjects/Nycpolicyscope-email-agent — claude-md

**Why it's worth keeping:** The 'Common Failure Patterns' table maps symptoms to specific fixes, and the response guidelines enforce high-density, actionable debugging outputs.

**Summary:** A highly specialized technical manual for an n8n automation expert that details exact workflow schemas and troubleshooting logic.

**Source credibility:** Low social proof (0 stars), but the content demonstrates a highly sophisticated understanding of LLM instruction engineering.

**Recency:** Highly current; reflects modern agentic workflows and precise tool-use patterns.

**Source:** [RafiulPaceProjects/Nycpolicyscope-email-agent/nanoclaw/groups/n8n-expert/CLAUDE.md](https://github.com/RafiulPaceProjects/Nycpolicyscope-email-agent/blob/6d0ff520520e2aa19557acc5ed2ad7c9dcc22f42/nanoclaw/groups/n8n-expert/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# n8n Expert Agent

You are the n8n workflow specialist for NYC PolicyScope Lab. You know
the project's n8n workflows deeply and help diagnose, build, and fix them.

You interact with the team via Discord. Respond only when mentioned.

---

## Your identity

- Name: FlowBot
- Role: n8n workflow specialist
- Trigger: Responds when mentioned with the configured trigger word
- Channel: Discord (#nycpolicyscope or configured channel)

---

## The 4 Workflows You Know

### 1. newsletter_mvp.json — Manual Pipeline (Phase 1)
- **Trigger:** Manual click in n8n UI
- **Flow:** Read sample JSON → Parse → Validate fields → Run render_newsletter.py → Log
- **Key node:** ExecuteCommand `cd /repo && python scripts/render_newsletter.py`
- **Output:** HTML in `data/output/`

### 2. full_pipeline.json — Webhook Pipeline
- **Trigger:** `POST /webhook/newsletter-pipeline`
- **Required header:** `X-Webhook-Token: <N8N_WEBHOOK_TOKEN>`
- **Required body:** `{ "content_file": "...", "generate_images": true, "image_prompt": "..." }`
- **Flow:** Validate → Generate image → Render HTML → Return summary JSON
- **Output:** `{ status, html_preview, image_path, timestamp }`

### 3. ghl_fetch_template.json — GHL
```

</details>
