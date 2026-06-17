---
name: Melkeydev__yappr
source: https://github.com/Melkeydev/yappr/blob/2dc524b890f56f283445c41f2f45d38ed642b08b/CLAUDE.md
repo: Melkeydev/yappr
kind: claude-md
stars: 122
last_pushed: 2026-02-08T02:32:24Z
license: mit
score: 8
domains: [backend-api, fullstack]
tags: [go, react, architecture]
curated: 2026-06-14
curated_by: config-scout
---

# Melkeydev/yappr — claude-md

**Why it's worth keeping:** Includes a 'Common Issues & Solutions' section for proactive debugging and a 'Testing Checklist' to guide agentic verification.

**Summary:** A high-density architectural blueprint that defines system constraints, database schema, and background job logic.

**Source credibility:** Legitimate real-world project with 122 stars and recent maintenance.

**Recency:** 

**Source:** [Melkeydev/yappr/CLAUDE.md](https://github.com/Melkeydev/yappr/blob/2dc524b890f56f283445c41f2f45d38ed642b08b/CLAUDE.md) · 122★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Go Chat App - Project Overview

## Architecture

### Backend (Go)
- **Framework**: Chi router with Gorilla WebSocket
- **Database**: PostgreSQL with automatic migrations
- **Authentication**: JWT tokens stored in HTTP-only cookies
- **Real-time**: WebSocket-based messaging with in-memory message history

### Frontend (React + TypeScript)
- **Build**: Vite
- **Styling**: Tailwind CSS
- **Forms**: react-hook-form
- **HTTP**: Axios with credentials

## Key Features

### 1. Room Management
- **24-hour expiration**: ALL rooms expire 24 hours after creation
- **Room limits**: 
  - Global limit: configurable via `MAX_ROOMS` env var (default: 50)
  - Per user limit: Logged-in users can only create 1 active room at a time
  - Anonymous users cannot create rooms
- **Database persistence**: Rooms and messages stored in PostgreSQL

### 2. User System
- **Authenticated users**: 
  - Can create one room at a time
  - Can change username via profile page
  - JWT authentication with 24-hour tokens
- **Anonymous users**:
  - Auto-generated username: `anonymousUser_[6-chars]`
  - Username persisted in localStorage
  - Cannot create rooms
  - Can join and chat in existing rooms

### 3. Pinned Topic
```

</details>
