---
name: caspii__dinkydash
source: https://github.com/caspii/dinkydash/blob/2a15df2e318f98ab229f097f84b5319f5686d7ae/CLAUDE.md
repo: caspii/dinkydash
kind: claude-md
stars: 91
last_pushed: 2026-02-28T20:44:26Z
license: unknown
score: 8
domains: [web-app, automation, python]
tags: [cron-job, llm-pipeline, flask]
curated: 2026-06-15
curated_by: config-scout
---

# caspii/dinkydash — claude-md

**Why it's worth keeping:** It explicitly explains the data lifecycle (the 'Two-Script Model') and details specific business logic like chore rotation algorithms, preventing AI hallucinations about how features function.

**Summary:** Defines a dual-process architecture where an LLM-driven cron job generates daily JSON content that is subsequently served via a Flask web app.

**Source credibility:** Strong; 91 stars indicates a functional, real-world utility.

**Recency:** Current; reflects modern development patterns for LLM-integrated automation.

**Source:** [caspii/dinkydash/CLAUDE.md](https://github.com/caspii/dinkydash/blob/2a15df2e318f98ab229f097f84b5319f5686d7ae/CLAUDE.md) · 91★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

DinkyDash is a family dashboard on a Raspberry Pi. A daily cron job calls the Claude API to generate personalized content based on a Google Calendar and family info. The Flask app renders the pre-generated JSON.

The project has two main components:
1. **Dashboard App** (root directory) - `generate.py` (daily content generation) + `app.py` (Flask server)
2. **Static Site Generator** (website/ directory) - Generates marketing/documentation site to GitHub Pages

## Development Commands

### Dashboard App

**Setup** (requires Python 3.11+)
```bash
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

**Generate dashboard content** (requires `ANTHROPIC_API_KEY` in `.env`):
```bash
python generate.py
```

**Run dev server**
```bash
flask run --host=0.0.0.0
```

**Deploy to Raspberry Pi**
```bash
./deploy_to_pi.sh
```

### Static Site Generator (Marketing Site)

**Build static site**
```bash
cd website
python build.py
```

## Architecture

### Two-Script Model

```
[cron @ 6am] -> generate.py -> fetches Google Calendar
```

</details>
