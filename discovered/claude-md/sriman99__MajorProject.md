---
name: sriman99__MajorProject
source: https://github.com/sriman99/MajorProject/blob/00972964a292f3f1d4331576a5f4b3c62ff08bfa/CLAUDE.md
repo: sriman99/MajorProject
kind: claude-md
stars: 2
last_pushed: 2026-04-22T19:51:22Z
license: mit
score: 9
domains: [backend-api, ml-ops, fullstack]
tags: [microservices, fastapi, react, ai-integration]
curated: 2026-06-15
curated_by: config-scout
---

# sriman99/MajorProject — claude-md

**Why it's worth keeping:** Includes specific 'Common Development Tasks' workflows and clear explanations of service interactions (ports, authentication flows, and the ML pipeline) which are vital for an agent.

**Summary:** A highly detailed guide for a multi-service healthcare platform involving AI/ML orchestration and real-time communication.

**Source credibility:** Low star count but demonstrates high-quality, manually authored technical documentation.

**Recency:** Current; uses modern stacks like React 19 and FastAPI.

**Source:** [sriman99/MajorProject/CLAUDE.md](https://github.com/sriman99/MajorProject/blob/00972964a292f3f1d4331576a5f4b3c62ff08bfa/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a healthcare management system focused on **respiratory disease detection** using AI/ML. The platform enables:
- AI-powered respiratory disease diagnosis from audio samples
- Real-time doctor-patient communication via WebSocket chat
- Appointment scheduling and management
- Multi-role user system (Admin, Doctor, Patient)

**Tech Stack:**
- **Frontend:** React 19 + TypeScript + Vite + TailwindCSS
- **Backend:** FastAPI (Python) + MongoDB
- **ML Service:** Separate FastAPI service with TensorFlow/Keras model
- **Real-time:** WebSocket for chat functionality

## Repository Structure

```
MajorProject/
├── backend/              # FastAPI backend (port 8000)
│   ├── main.py          # Main API with auth, CRUD, WebSocket
│   ├── websocket_manager.py  # WebSocket connection handling
│   ├── middleware.py    # Auth middleware
│   ├── init_db.py       # Database initialization
│   ├── seed_data.py     # Sample data seeding
│   └── uploads/         # Audio file storage
├── ml_model/            # ML inference service (port 8001)
│   ├── main.py
```

</details>
