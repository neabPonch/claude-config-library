---
name: olavolicursi__Finanpy
source: https://github.com/olavolicursi/Finanpy/blob/6cac48b452c49e21535d1766ed12b648a72fb780/CLAUDE.MD
repo: olavolicursi/Finanpy
kind: claude-md
stars: 0
last_pushed: 2026-02-21T21:45:20Z
license: mit
score: 7
domains: [web-backend, django]
tags: [monolith, architecture-mapping, coding-conventions]
curated: 2026-06-16
curated_by: config-scout
---

# olavolicursi/Finanpy — claude-md

**Why it's worth keeping:** The explicit definition of module responsibilities and Django design patterns (like logic placement and query optimization) prevents the AI from generating generic or inconsistent code.

**Summary:** Provides essential project mapping, tech stack versions, and specific implementation guidelines.

**Source credibility:** Personal repository with no social proof or significant history.

**Recency:** 

**Source:** [olavolicursi/Finanpy/CLAUDE.MD](https://github.com/olavolicursi/Finanpy/blob/6cac48b452c49e21535d1766ed12b648a72fb780/CLAUDE.MD) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Finanpy Context for Gemini

This file provides context for the Finanpy project, a Personal Finance Management System.

## Project Overview

**Finanpy** is a web-based application for managing personal finances. It allows users to control bank accounts, categorize transactions (incomes and expenses), and view financial dashboards.

*   **Status**: Active Development (Sprint 1 - Configuration & Authentication).
*   **Key Documentation**:
    *   `PRD.MD`: Product Requirements Document (detailed features, user stories, schema).
    *   `docs/`: Contains architecture, database, design system, and setup guides.

## Architecture

The project follows a **Monolithic Django** architecture.

### Directory Structure
*   **`core/`**: Project settings, URLs, ASGI/WSGI configuration.
*   **`users/`**: Custom user model and authentication logic.
*   **`accounts/`**: Management of bank accounts.
*   **`categories/`**: Transaction categories (income/expense).
*   **`transactions/`**: Core transaction logic (recording incomes/expenses).
*   **`profiles/`**: User profiles (avatar, bio).
*   **`docs/`**: Project documentation.

### Tech Stack
*   **Backend**: Python 3.12+, Django 6.0.1.
*   **Databa
```

</details>
