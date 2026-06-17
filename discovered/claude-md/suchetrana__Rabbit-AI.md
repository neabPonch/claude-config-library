---
name: suchetrana__Rabbit-AI
source: https://github.com/suchetrana/Rabbit-AI/blob/bf9302f32dbbc96e836cfe10864751c8a0b12aba/Claude.md
repo: suchetrana/Rabbit-AI
kind: claude-md
stars: 0
last_pushed: 2026-03-11T13:12:31Z
license: unknown
score: 8
domains: [ai-agents, mcp-integration, web-development]
tags: [mcp, prompt-engineering, fullstack]
curated: 2026-06-14
curated_by: config-scout
---

# suchetrana/Rabbit-AI — claude-md

**Why it's worth keeping:** It includes specific 'How to Use' prompt templates that teach the AI agent how to interact with tools; it also uses structured tables for security and deployment context.

**Summary:** A highly practical guide that combines project structure with deep, prompt-based instructions for utilizing an external MCP tool (Google Stitch).

**Source credibility:** Low social proof via GitHub, but high technical sophistication in documentation style.

**Recency:** Very recent; demonstrates modern MCP-centric development patterns.

**Source:** [suchetrana/Rabbit-AI/Claude.md](https://github.com/suchetrana/Rabbit-AI/blob/bf9302f32dbbc96e836cfe10864751c8a0b12aba/Claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — Rabbitt Sales Insight Automator

> This file persists project context across Claude sessions.
> Read this file at the start of every session before making any changes.

---

## 📦 Project Overview

**Project Name:** Rabbitt Sales Insight Automator  
**Role:** AI Cloud DevOps Engineer  
**Stack:** React + Vite (Frontend) · Node.js + Express (Backend)  
**Goal:** Upload CSV/XLSX sales data → AI generates summary → Email delivered to recipient

---

## 🗂️ Project Structure

```
rabbitt-sales-insight/
├── frontend/                    # React + Vite → deploy on Vercel
│   ├── src/
│   │   ├── components/          # UploadForm, FileDropzone, StatusBanner
│   │   ├── hooks/               # useUpload.js
│   │   ├── services/            # api.js (Axios instance)
│   │   ├── App.jsx
│   │   └── main.jsx
│   ├── Dockerfile
│   └── .env.example
│
├── backend/                     # Node.js + Express → deploy on Render
│   ├── src/
│   │   ├── config/              # env.js (dotenv + Zod validation)
│   │   ├── middlewares/         # rateLimiter, helmet, validate, errorHandler
│   │   ├── routes/              # upload.route.js
│   │   ├── controllers/         # upload.controller.js
│
```

</details>
