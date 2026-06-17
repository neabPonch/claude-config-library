---
name: AbdulazizYas__Quarch
source: https://github.com/AbdulazizYas/Quarch/blob/4553c99077917bc4104276802a4fd66dde86455d/CLAUDE.md
repo: AbdulazizYas/Quarch
kind: claude-md
stars: 0
last_pushed: 2026-04-15T17:17:29Z
license: unknown
score: 9
domains: [web-frontend, backend-api, fullstack]
tags: [architectural-patterns, data-flow, implementation-recipes]
curated: 2026-06-15
curated_by: config-scout
---

# AbdulazizYas/Quarch — claude-md

**Why it's worth keeping:** The inclusion of 'Data Flow Patterns' and 'Common Development Patterns' provides the AI with logical recipes rather than just static descriptions. It also includes high-value technical caveats (like node positioning math) that prevent logic errors during refactoring.

**Summary:** A highly detailed full-stack guide that maps out complex state management, data flows, and API structures.

**Source credibility:** Single-developer project with low social proof but exceptionally high documentation quality.

**Recency:** Very current, pushed within the last 2 months.

**Source:** [AbdulazizYas/Quarch/CLAUDE.md](https://github.com/AbdulazizYas/Quarch/blob/4553c99077917bc4104276802a4fd66dde86455d/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Quarch is a quantum circuit simulator with a React/TypeScript frontend and Python/FastAPI backend. It provides a visual drag-and-drop interface for building quantum circuits, simulating them with Qiskit, and creating reusable multi-qubit blocks.

## Development Commands

### Frontend (React + Vite + TypeScript)
```bash
cd frontend
npm install           # Install dependencies (one time)
npm run dev           # Start dev server on http://localhost:5173
npm run build         # Build for production (runs TypeScript compiler + Vite build)
npm run lint          # Run ESLint
npm run preview       # Preview production build
```

### Backend (Python + FastAPI + Qiskit)
```bash
cd backend

# Setup (one time)
python -m venv venv
venv\Scripts\activate          # Windows
source venv/bin/activate       # Mac/Linux
pip install -r requirements.txt

# Running
python run.py          # Start server on http://localhost:8000 with auto-reload

# API Documentation
# Open http://localhost:8000/api/docs (Swagger UI)
# Open http://localhost:8000/api/redoc (ReDoc)
```

###
```

</details>
