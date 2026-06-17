---
name: semaphore-chat__semaphore-chat
source: https://github.com/semaphore-chat/semaphore-chat/blob/c035c32c3e2cf12f6802fff86b4bd3b428963ff9/CLAUDE.md
repo: semaphore-chat/semaphore-chat
kind: claude-md
stars: 18
last_pushed: 2026-06-13T01:46:18Z
license: agpl-3.0
score: 9
domains: [web-frontend, fullstack, docker-orchestration, desktop-app]
tags: [platform-separation, docker-first, architecture-patterns, api-regeneration]
curated: 2026-06-15
curated_by: config-scout
---

# semaphore-chat/semaphore-chat — claude-md

**Why it's worth keeping:** The 'Correct/Wrong' examples provide high-signal structural guardrails that prevent the AI from introducing messy platform checks, while the detailed command mapping ensures all actions happen inside containers.

**Summary:** This file provides strict environmental guardrails for Docker-centric development and explicit architectural patterns for cross-platform (Web vs Electron) code separation.

**Source credibility:** High; based on a real-world, specialized voice/video project with active development.

**Recency:** Current; reflects modern fullstack workflows involving Docker and OpenAPI spec synchronization.

**Source:** [semaphore-chat/semaphore-chat/CLAUDE.md](https://github.com/semaphore-chat/semaphore-chat/blob/c035c32c3e2cf12f6802fff86b4bd3b428963ff9/CLAUDE.md) · 18★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Documentation

Project documentation: [docs.semaphorechat.app](https://docs.semaphorechat.app) (source: `docs-site/`).

## 🐳 **CRITICAL**: ALL DEVELOPMENT USES DOCKER

**Never run pnpm/npm/yarn/node commands directly on the host. Always use Docker containers as shown in the Development Commands section below.**

## Project Overview

**Semaphore Chat** is a self-hosted voice and text chat application built with NestJS backend and React frontend.

### Core Concepts

- **Instance**: The application stack running in hosted or self-hosted environments
- **Communities**: User/admin-created servers with members, channels, and voice/video contexts
- **Members**: Users registered with the instance and added to communities
- **Channels**: Text and voice channels within communities
- **Direct Messages & Groups**: Private messaging between users (✅ implemented with file attachments)

### Platform Goals

- **Current**: Browser-based application
- **Future Roadmap**:
  - Mobile app (React Native or Electron)
  - Desktop application (Electron)

### Key Features

- Real-time mess
```

</details>
