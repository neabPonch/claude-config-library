---
name: LianjiaTech__bella-openapi
source: https://github.com/LianjiaTech/bella-openapi/blob/dc76eeab36ab8adca6ac7dbb8f050329407e1daf/CLAUDE.md
repo: LianjiaTech/bella-openapi
kind: claude-md
stars: 232
last_pushed: 2026-05-27T13:10:49Z
license: mit
score: 9
domains: [backend-api, ai-infrastructure, java-spring-boot, nextjs]
tags: [architecture-overview, workflow-recipes, production-grade]
curated: 2026-06-14
curated_by: config-scout
---

# LianjiaTech/bella-openapi — claude-md

**Why it's worth keeping:** It excels at explaining complex architectural patterns like the Protocol Adapter Pattern and provides explicit 'how-to' recipes for extending the system. The inclusion of request flows and debugging/logging configurations is highly effective for agentic troubleshooting.

**Summary:** Provides a comprehensive technical blueprint of an AI gateway, covering system architecture, command-line workflows, and specific feature extension steps.

**Source credibility:** High; 232 stars and documented as a production-grade system serving millions at Beike (KE Holdings).

**Recency:** Current; uses modern patterns like Next.js App Router and provides granular command structures perfect for Claude Code.

**Source:** [LianjiaTech/bella-openapi/CLAUDE.md](https://github.com/LianjiaTech/bella-openapi/blob/dc76eeab36ab8adca6ac7dbb8f050329407e1daf/CLAUDE.md) · 232★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Bella OpenAPI is an AI API gateway that provides unified access to multiple AI services (chat completion, embeddings, ASR, TTS, image generation). It's a production-grade system serving 150M+ daily API calls at Beike (KE Holdings). The project consists of a Java Spring Boot backend (api/) and a Next.js frontend (web/), deployed via Docker.

## Common Development Commands

### Docker Deployment (Recommended)
```bash
# Start all services with Docker
./start.sh

# Start with specific configurations
./start.sh --build                    # Rebuild services
./start.sh --rebuild                  # Force rebuild without cache
./start.sh --nginx-port 8080         # Use custom port
./start.sh --server https://domain.com  # Set server domain
./start.sh --skip-auth               # Skip admin authorization

# OAuth configuration
./start.sh --github-oauth CLIENT_ID:SECRET --google-oauth CLIENT_ID:SECRET

# Stop services
./stop.sh
```

### Backend API Development (Java/Maven)
```bash
cd api/

# Build the project
mvn clean compile
mvn clean package -DskipTests
```

</details>
