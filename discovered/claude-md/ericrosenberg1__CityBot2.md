---
name: ericrosenberg1__CityBot2
source: https://github.com/ericrosenberg1/CityBot2/blob/8742c87593af24e69b11b67d2fb2b9a5ef2ca8c2/CLAUDE.md
repo: ericrosenberg1/CityBot2
kind: claude-md
stars: 37
last_pushed: 2026-06-04T17:41:47Z
license: gpl-3.0
score: 7
domains: [python, bots, backend-api]
tags: [async, automation, python]
curated: 2026-06-14
curated_by: config-scout
---

# ericrosenberg1/CityBot2 — claude-md

**Why it's worth keeping:** The custom shell command for rapid syntax validation via py_compile and the rule to limit edits to files within a stack trace are excellent agent-specific instructions.

**Summary:** Defines an async Python bot stack with specific guardrails for error handling and syntax verification.

**Source credibility:** Small but active repository with recent maintenance.

**Recency:** Highly current; provides tool-centric instructions tailored for CLI-based AI agents.

**Source:** [ericrosenberg1/CityBot2/CLAUDE.md](https://github.com/ericrosenberg1/CityBot2/blob/8742c87593af24e69b11b67d2fb2b9a5ef2ca8c2/CLAUDE.md) · 37★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CityBot2 — Claude Code Instructions

## Tech stack
- Python async bot monitoring Ventura, CA (weather, earthquakes, news) and posting to social media
- FastAPI web dashboard (`web/app.py`)
- SQLAlchemy models in `database/models.py`

## Auto-fix guidelines
- **Test command:** `python -m py_compile $(find . -name "*.py" ! -path "./.git/*" | tr "\n" " ") && echo "Syntax OK"`
- No pytest suite — syntax check only
- Only modify the file shown in the stack trace
- Do not modify `config/cities/*.json` for code bugs
- Async/await throughout — maintain async consistency
- Env vars from `config/credentials.env.example` pattern (never hardcode)

## File map
- `main.py` — entry point
- `monitors/` — earthquake, weather, news polling
- `social_media/platforms/` — Bluesky, Twitter, Reddit, etc.
- `web/app.py` — FastAPI admin dashboard
- `database/models.py` — SQLAlchemy models
```

</details>
