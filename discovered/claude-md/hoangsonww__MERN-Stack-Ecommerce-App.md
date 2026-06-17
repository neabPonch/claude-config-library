---
name: hoangsonww__MERN-Stack-Ecommerce-App
source: https://github.com/hoangsonww/MERN-Stack-Ecommerce-App/blob/6b1c21466b192f53724e6ea9d6622b6c0cbb0eed/CLAUDE.md
repo: hoangsonww/MERN-Stack-Ecommerce-App
kind: claude-md
stars: 117
last_pushed: 2026-06-15T00:28:51Z
license: mit
score: 9
domains: [web-frontend, backend-api, ai-integration, ecommerce]
tags: [mern, vector-search, monorepo, architecture-pattern]
curated: 2026-06-16
curated_by: config-scout
---

# hoangsonww/MERN-Stack-Ecommerce-App — claude-md

**Why it's worth keeping:** It includes detailed 'Critical Data Flow' explanations and specific warnings about automated side effects (Mongoose hooks), which prevents an AI from accidentally breaking the vector sync logic.

**Summary:** A high-quality guide for a MERN stack application integrated with vector databases for AI recommendations. It covers architecture, data synchronization patterns, and specific operational commands.

**Source credibility:** 117 stars and recently updated; a well-maintained sample project.

**Recency:** Current; utilizes modern stacks including React Router v6 and various Vector DBs.

**Source:** [hoangsonww/MERN-Stack-Ecommerce-App/CLAUDE.md](https://github.com/hoangsonww/MERN-Stack-Ecommerce-App/blob/6b1c21466b192f53724e6ea9d6622b6c0cbb0eed/CLAUDE.md) · 117★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**Fusion Electronics** is a production-ready MERN stack e-commerce application with AI-powered product recommendations using vector databases (Pinecone, Weaviate, FAISS). The project consists of a React frontend, Express.js backend, MongoDB database, and vector database integrations for semantic product search and recommendations.

## Essential Commands

### Development Setup

```bash
# Install dependencies
npm install                          # Frontend
cd backend && npm install            # Backend

# Database seeding
cd backend/seed && node productSeeds.js dev

# Sync vector databases (required for recommendations)
cd backend && npm run sync-pinecone  # Primary vector DB
```

### Running the Application

```bash
# Development mode - both servers concurrently
npm run dev

# Or run separately:
npm start                            # Frontend (port 3000)
cd backend && npm start              # Backend (port 5000)
```

### Testing

```bash
# Frontend tests
npm test                             # Run all tests
npm run test:watch                   # Wa
```

</details>
