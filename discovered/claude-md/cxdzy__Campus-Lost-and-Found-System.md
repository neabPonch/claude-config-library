---
name: cxdzy__Campus-Lost-and-Found-System
source: https://github.com/cxdzy/Campus-Lost-and-Found-System/blob/78901f58b93dacd27877993f23cbf81f90a31252/CLAUDE.md
repo: cxdzy/Campus-Lost-and-Found-System
kind: claude-md
stars: 0
last_pushed: 2026-06-16T13:14:41Z
license: unknown
score: 9
domains: [backend-api, system-architecture, ai-integration]
tags: [laravel, service-orchestration, api-contracts, bot-driven]
curated: 2026-06-16
curated_by: config-scout
---

# cxdzy/Campus-Lost-and-Found-System — claude-md

**Why it's worth keeping:** It defines strict cross-service boundaries (PHP vs Node.js) to prevent logic leakage and provides explicit API request/response contracts including required security headers.

**Summary:** An architectural guide for a multi-service system involving a Laravel API and a separate Node.js Telegram bot. It outlines exact service boundaries, API contracts, and complex data workflows.

**Source credibility:** Low star count suggests a niche or academic project, but the documentation depth is highly professional.

**Recency:** Highly current; uses modern deployment tools like Dokploy and integration patterns suitable for today's AI agents.

**Source:** [cxdzy/Campus-Lost-and-Found-System/CLAUDE.md](https://github.com/cxdzy/Campus-Lost-and-Found-System/blob/78901f58b93dacd27877993f23cbf81f90a31252/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

Guidance for AI coding agents (Claude Code / VS Code) working in this repository.

---

## 1. Project Overview

**Campus Lost & Found** is an AI-powered, back-end-driven system that modernizes the manual
lost-and-found process on the UiTM campus. It replaces paper logbooks and notice boards with an
automated recovery pipeline built around a **Laravel back-end** orchestrating vision analysis,
spatial matching, and Telegram notifications.

The defining feature is **AI Vision + spatial matching**: when a "Found" item is reported via the
Telegram bot, the system extracts visual tags via **Google Cloud Vision API** and stores GPS coordinates. A matching engine compares tags + proximity against Lost reports. A notification fires
only when the confidence score exceeds the configured threshold (default 80%).

- **Course context:** ITT626 — Back-End Technology
- **Deployment:** Self-hosted VPS managed with **Dokploy** — Laravel app, Node.js bot, and
  PostgreSQL each run as separate Dokploy services
- **Primary frontends:** Telegram Bot (Node.js/Telegraf, separate GitHub repo) + Vue.js SPA via Inertia.js (web)

---

## 2. Tech Stack

| Layer | Technology |
|-------|-----------|
```

</details>
