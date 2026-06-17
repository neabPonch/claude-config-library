---
name: mimo-x__Code-Review-GPT-Gitlab
source: https://github.com/mimo-x/Code-Review-GPT-Gitlab/blob/aff1e87be8d8cc0dd7679b1300157c55600cf187/CLAUDE.md
repo: mimo-x/Code-Review-GPT-Gitlab
kind: claude-md
stars: 820
last_pushed: 2025-12-05T10:41:39Z
license: mit
score: 8
domains: [backend, frontend, ai-integration, fullstack]
tags: [django, vuejs, architecture-map, workflow-logic]
curated: 2026-06-14
curated_by: config-scout
---

# mimo-x/Code-Review-GPT-Gitlab — claude-md

**Why it's worth keeping:** Excellent use of 'Key Application Flow' to explain logic paths and 'Development Notes' to document subtle nuances like timezones and mock modes.

**Summary:** A comprehensive full-stack guide mapping a Django/Vue.js architecture with clear data flows and command sets.

**Source credibility:** Highly credible source; 820 stars indicates a widely used tool in the GitLab ecosystem.

**Recency:** Very current, pushed within the last 6 months.

**Source:** [mimo-x/Code-Review-GPT-Gitlab/CLAUDE.md](https://github.com/mimo-x/Code-Review-GPT-Gitlab/blob/aff1e87be8d8cc0dd7679b1300157c55600cf187/CLAUDE.md) · 820★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

# 当我没有在书面上请求你生成任何说明文档的时候，禁止你生成任何说明文档

## Project Overview

Code Review GPT GitLab is a Django + Vue.js full-stack application that automates code review using Large Language Models (LLMs). It integrates with GitLab via webhooks and supports 40+ LLM providers through UnionLLM.

## Development Commands

### Backend (Django)
```bash
# Development server
python manage.py runserver 0.0.0.0:8000
./start.sh                   # Automated development startup

# Database
python manage.py migrate    # Run migrations
python manage.py createsuperuser  # Admin user

# Production
./start_production.sh       # Production deployment with gunicorn
gunicorn core.wsgi:application --bind 0.0.0.0:8000 --workers 4 --worker-class gevent

# Docker
docker compose up -d        # Build backend image + start stack
```

### Frontend (Vue.js)
```bash
npm install                 # Install dependencies
npm run dev                 # Development server (localhost:3000)
npm run build              # Production build
npm run preview            # Preview production build
```

## Architecture

### Backend
```

</details>
