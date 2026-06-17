---
name: tryvinci__vinci-clips
source: https://github.com/tryvinci/vinci-clips/blob/d344eefea3af4995444ef8594910d00dbc72a78e/CLAUDE.md
repo: tryvinci/vinci-clips
kind: claude-md
stars: 124
last_pushed: 2026-02-14T09:01:42Z
license: other
score: 8
domains: [web-frontend, backend-api, ai-services]
tags: [architecture-focused, roadmap-driven, multi-service]
curated: 2026-06-16
curated_by: config-scout
---

# tryvinci/vinci-clips — claude-md

**Why it's worth keeping:** The 'Current Development Status' section provides vital context for agentic task planning, while the breakdown of specific shell commands eliminates guesswork during environment setup.

**Summary:** A comprehensive architectural guide featuring explicit development commands for a multi-service stack and an detailed project roadmap.

**Source credibility:** Active open-source project with recent activity and moderate star count.

**Recency:** Highly current; references modern technologies like Next.js App Router and Turbopack.

**Source:** [tryvinci/vinci-clips/CLAUDE.md](https://github.com/tryvinci/vinci-clips/blob/d344eefea3af4995444ef8594910d00dbc72a78e/CLAUDE.md) · 124★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Vinci Clips is an AI-powered video clipping tool that automatically generates short, engaging video clips from longer videos. The application uses AI to transcribe videos, analyze transcripts, and suggest the best moments to turn into clips.

**Architecture:**
- **Frontend:** Next.js application with React, TypeScript, and Tailwind CSS
- **Backend:** Node.js/Express REST API server
- **Database:** MongoDB with Mongoose ODM
- **AI Services:** Google Gemini API for transcription and analysis
- **Cloud Storage:** Google Cloud Storage for video/audio files
- **Video Processing:** FFmpeg for video-to-audio conversion and caption burning

## Development Commands

### Root Level Commands
```bash
# Install dependencies for both frontend and backend
npm run install:all

# Start both frontend and backend concurrently
npm start

# Start only backend (runs on port 8080)
npm run start:backend

# Start only frontend (runs on port 3000)
npm run start:frontend
```

### Backend Commands (from /backend directory)
```bash
# Start production server
npm start

# Star
```

</details>
