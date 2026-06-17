---
name: zuocharles__openclaw-social-media-skill
source: https://github.com/zuocharles/openclaw-social-media-skill/blob/85ed2f4dabd47ffbe7743556d1f3be2db36ca43b/skill.md
repo: zuocharles/openclaw-social-media-skill
kind: skill
stars: 4
last_pushed: 2026-02-17T21:59:47Z
license: mit
score: 8
domains: [agents-ai, cli-tools, web-scraping]
tags: [social-media, research, discovery, automation]
curated: 2026-06-14
curated_by: config-scout
---

# zuocharles/openclaw-social-media-skill — skill

**Why it's worth keeping:** Excellent templates for agentic state management (HEARTBEAT/SOUL files) and proactive error handling for session expirations.

**Summary:** A comprehensive skill guide for social media discovery that includes patterns for integrating findings into an agent's long-term memory and lifecycle.

**Source credibility:** 4 stars; highly structured documentation indicates a sophisticated understanding of autonomous workflows.

**Recency:** Highly current, with updates through February 2026.

**Source:** [zuocharles/openclaw-social-media-skill/skill.md](https://github.com/zuocharles/openclaw-social-media-skill/blob/85ed2f4dabd47ffbe7743556d1f3be2db36ca43b/skill.md) · 4★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Social Media Search Skill

Search X/Twitter and LinkedIn for mentions, use cases, pain points, and trending topics.

**Cost:** $0/month (vs $200/month for Twitter API)

---

## When to Use This Skill

Use this skill when you need to:
- 🔍 **Discover use cases** - See what people are building with your product
- 💬 **Find mentions** - Track what people say about your product
- 😫 **Identify pain points** - See what problems people are struggling with
- 📈 **Monitor trends** - Track trending topics in your space
- 🤝 **Find collaborators** - Discover people working on similar projects
- 📊 **Market research** - Understand what your audience cares about

**Do NOT use this for:**
- Posting to social media (this is read-only)
- Real-time monitoring (sessions expire every ~30 days)
- High-frequency searches (keep it reasonable, 100-200/day max)

---

## How to Use

### Basic Search

```bash
python3 ~/.openclaw/tools/agent-social-search.py "your search query"
```

**Returns JSON:**
```json
{
  "query": "OpenClaw",
  "x_results": [
    {
      "platform": "X",
      "text": "Tweet content...",
      "username": "username",
      "url": "https://x.com/username/status/123...",
      "index": 1
```

</details>
