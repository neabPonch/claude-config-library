---
name: gessnerfl__fake-smtp-server
source: https://github.com/gessnerfl/fake-smtp-server/blob/13475ff497e42a9b728606558fb9479498460f4c/CLAUDE.md
repo: gessnerfl/fake-smtp-server
kind: claude-md
stars: 503
last_pushed: 2026-06-04T02:25:28Z
license: apache-2.0
score: 9
domains: [fullstack, java, react]
tags: [spring-boot, smtp, api-integration]
curated: 2026-06-15
curated_by: config-scout
---

# gessnerfl/fake-smtp-server — claude-md

**Why it's worth keeping:** Excellent use of 'Core Flow' descriptions that explain how data moves through the system, which is vital for agentic reasoning beyond simple file reading.

**Summary:** Provides highly structured architectural context, specific command groupings, and detailed data flow mapping for a full-stack application.

**Source credibility:** High; well-maintained project with significant GitHub stars (503).

**Recency:** Current; includes modern stack context like React 19 and Vite.

**Source:** [gessnerfl/fake-smtp-server/CLAUDE.md](https://github.com/gessnerfl/fake-smtp-server/blob/13475ff497e42a9b728606558fb9479498460f4c/CLAUDE.md) · 503★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Fake SMTP Server is a Java Spring Boot application with a React frontend that provides a development SMTP server for testing email functionality. It captures emails in-memory and displays them through a web interface instead of actually sending them.

## Architecture

### Backend (Spring Boot)
- **Main Package**: `de.gessnerfl.fakesmtp`
- **SMTP Server**: Custom SMTP implementation in `smtp/` package with command handlers, authentication, and message processing
- **Data Layer**: JPA entities and repositories for email storage with H2 in-memory database
- **REST API**: Controllers in `controller/` package expose email management endpoints
- **Configuration**: Properties-based configuration in `config/` package for SMTP settings, authentication, TLS

### Frontend (React)
- **Location**: `webapp/` directory
- **Stack**: React 19, TypeScript, Material-UI, Redux Toolkit, Vite
- **Pages**: Email list and detail views with search/filtering capabilities
- **State**: RTK Query for API communication with backend REST endpoints

### Integration
- Frontend b
```

</details>
