---
name: kevinsinghdeveloper__ToStructuredAI
source: https://github.com/kevinsinghdeveloper/ToStructuredAI/blob/a2e2030872c0e6efa5413893906c3ece4137999d/claude.md
repo: kevinsinghdeveloper/ToStructuredAI
kind: claude-md
stars: 0
last_pushed: 2026-04-17T02:41:40Z
license: unknown
score: 9
domains: [fullstack, architectural-patterns, web-app]
tags: [architecture-blueprints, workflow-automation]
curated: 2026-06-16
curated_by: config-scout
---

# kevinsinghdeveloper/ToStructuredAI — claude-md

**Why it's worth keeping:** The 'Key Files to Edit' mapping and the explicit enforcement of the Controller-Manager-Service pattern are highly transferable techniques for maintaining structural consistency.

**Summary:** Provides high-density architectural context for a full-stack application including layer definitions and state management rules.

**Source credibility:** Low social proof (0 stars), but the documentation structure suggests a sophisticated developer-led project.

**Recency:** Highly current, utilizing modern stacks like React 18 and MUI v5.

**Source:** [kevinsinghdeveloper/ToStructuredAI/claude.md](https://github.com/kevinsinghdeveloper/ToStructuredAI/blob/a2e2030872c0e6efa5413893906c3ece4137999d/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Code Instructions - Zerve App

## Quick Commands

```bash
# Frontend
cd frontend && npm install && npm start    # Dev server on http://localhost:3000

# Backend
cd backend && pip install -r requirements.txt && python run_web_service.py  # API on http://localhost:8000

# Full stack (Docker)
docker-compose up --build    # Frontend :3000, Backend :8000, PostgreSQL :5432
```

## Project Structure

```
zerve-app/
  frontend/                # React 18 + TypeScript + MUI + Tailwind
    src/
      components/
        context_providers/ # React Context (Auth, User, RBAC, Theme, Documents, Notification)
        pages/             # Page components
        shared/            # Shared components (Header, Footer, ProtectedRoute, LoadingSpinner)
      utils/               # API service layer (Axios)
      configs/             # API endpoints configuration
      types/               # TypeScript type definitions
      theme/               # MUI theme configuration
  backend/                 # Flask + SQLAlchemy + LangChain
    abstractions/          # Base classes (IController, IResourceManager, IServiceManagerBase)
    controllers/           # HTTP route handlers (thin layer)
    manage
```

</details>
