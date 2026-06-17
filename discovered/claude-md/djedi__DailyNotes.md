---
name: djedi__DailyNotes
source: https://github.com/djedi/DailyNotes/blob/22f2168a8dfc3cffc5e6fdb8bdf79e1ff277cbd7/CLAUDE.md
repo: djedi/DailyNotes
kind: claude-md
stars: 712
last_pushed: 2026-05-22T21:30:45Z
license: mit
score: 9
domains: [fullstack, web-app, security]
tags: [architecture, context-rich]
curated: 2026-06-15
curated_by: config-scout
---

# djedi/DailyNotes — claude-md

**Why it's worth keeping:** It explains 'how' the system works (data movement and security) rather than just listing files, which allows an AI to reason about side effects and complex changes.

**Summary:** Provides high-density architectural context including data flow logic, encryption strategies, and specific component relationships.

**Source credibility:** High; a popular open-source project with 700+ stars and recent maintenance.

**Recency:** Highly current; provides the high-level abstraction necessary for modern agentic coding workflows.

**Source:** [djedi/DailyNotes/CLAUDE.md](https://github.com/djedi/DailyNotes/blob/22f2168a8dfc3cffc5e6fdb8bdf79e1ff277cbd7/CLAUDE.md) · 712★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# DailyNotes Architecture Guide

## Important Rules

- **Never commit unless explicitly told to.** Wait for the user to ask you to commit changes.

## Project Overview

DailyNotes is a self-hosted daily task and note-taking application that combines the experience of a physical planner with modern web technology. It supports markdown with GitHub Flavored Markdown (GFM) task lists, making it ideal for daily journaling, task tracking, and note management.

**Version Format:** `YYYY.MM.DD-##` (date-based with daily build number, managed by CI)

## Technology Stack

### Backend

- **Framework:** Quart (async Python microframework, Flask-compatible)
- **Database ORM:** SQLAlchemy (raw, without Flask-SQLAlchemy)
- **Authentication:** JWT (JSON Web Tokens) via PyJWT with custom decorators
- **Password Hashing:** Argon2 via argon2-cffi
- **Database Migrations:** Alembic
- **Production Server:** Uvicorn (ASGI)
- **HTTP Client:** httpx (async HTTP requests)
- **Data Encryption:** PyCryptodome (AES encryption for sensitive data at rest)
- **Markdown Processing:** python-frontmatter (for parsing YAML frontmatter)

**Python Version:** Python 3.8+

### Frontend

- **Framework:** Vue.js 2.6
- **L
```

</details>
