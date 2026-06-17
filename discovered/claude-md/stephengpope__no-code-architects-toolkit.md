---
name: stephengpope__no-code-architects-toolkit
source: https://github.com/stephengpope/no-code-architects-toolkit/blob/d9bb5679e203e6b5d3b3c2b9ab848a289c645024/CLAUDE.md
repo: stephengpope/no-code-architects-toolkit
kind: claude-md
stars: 2308
last_pushed: 2026-01-02T01:51:53Z
license: gpl-2.0
score: 9
domains: [backend-api, media-processing]
tags: [flask, api-architecture, task-queueing]
curated: 2026-06-15
curated_by: config-scout
---

# stephengpope/no-code-architects-toolkit — claude-md

**Why it's worth keeping:** Includes highly actionable 'Adding New Features' workflows and explicit code templates for the blueprint/service pattern, ensuring architectural consistency when extending the app.

**Summary:** Documents a complex Flask media processing API that utilizes custom decorators for task queueing, GCP Cloud Run jobs, and cloud storage abstraction.

**Source credibility:** High; sourced from a popular toolkit with over 2,300 stars.

**Recency:** Current; follows modern Python/Flask patterns ideal for AI-assisted development.

**Source:** [stephengpope/no-code-architects-toolkit/CLAUDE.md](https://github.com/stephengpope/no-code-architects-toolkit/blob/d9bb5679e203e6b5d3b3c2b9ab848a289c645024/CLAUDE.md) · 2308★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

No-Code Architects Toolkit API is a Flask-based media processing API that handles audio/video conversion, transcription, translation, captioning, and cloud storage integration. It supports deployment on Docker, Google Cloud Platform, and Digital Ocean.

## Architecture

### Core Components

- **[app.py](app.py)** - Main Flask application with queue-based task processing
  - Creates task queue for async job processing
  - Provides `queue_task` decorator for route handlers
  - Supports GCP Cloud Run Jobs for long-running tasks
  - Auto-registers blueprints from `routes/` directory

- **[app_utils.py](app_utils.py)** - Core utilities
  - `validate_payload()` - JSON schema validation decorator
  - `queue_task_wrapper()` - Wraps routes for queue processing
  - `discover_and_register_blueprints()` - Auto-discovers and registers Flask blueprints
  - `log_job_status()` - Logs job status to LOCAL_STORAGE_PATH/jobs

- **[config.py](config.py)** - Environment configuration
  - Validates required environment variables per storage provider
  - Configures API_KEY, sto
```

</details>
