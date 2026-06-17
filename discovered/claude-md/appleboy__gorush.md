---
name: appleboy__gorush
source: https://github.com/appleboy/gorush/blob/52b6914fb41cb6b4b00d2b8d2547effa1fe1bf5c/CLAUDE.md
repo: appleboy/gorush
kind: claude-md
stars: 8737
last_pushed: 2026-06-13T15:55:10Z
license: mit
score: 9
domains: [backend, go, api]
tags: [architecture-mapping, system-design]
curated: 2026-06-15
curated_by: config-scout
---

# appleboy/gorush — claude-md

**Why it's worth keeping:** The 'Request Flow' section is an elite technique for teaching LLMs system logic, and providing exact build tags/environment variables prevents command failures during automated tasks.

**Summary:** This file provides a detailed architectural map of how data flows through the system alongside specific development workflows.

**Source credibility:** Very high; the source repo is a well-starred, actively maintained Go project.

**Recency:** Current; it offers specific operational context that modern AI coding agents need to navigate complex build processes.

**Source:** [appleboy/gorush/CLAUDE.md](https://github.com/appleboy/gorush/blob/52b6914fb41cb6b4b00d2b8d2547effa1fe1bf5c/CLAUDE.md) · 8737★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Gorush is a push notification microserver written in Go that supports sending notifications to iOS (APNS), Android (FCM), and Huawei (HMS) devices. It provides both HTTP REST API and gRPC interfaces.

## Architecture

### Request Flow

1. **main.go** parses CLI flags, loads config, initializes platform clients (APNS/FCM/HMS), then starts HTTP (Gin) and gRPC servers via `graceful.Manager`
2. **router/** receives push requests at `POST /api/push`, validates them, and enqueues `PushNotification` messages into the queue
3. **app/worker.go** creates the queue worker (local/NSQ/NATS/Redis) with `notify.Run(cfg)` as the processing function
4. **notify/** dispatches notifications to platform-specific push functions (`PushToIOS`, `PushToAndroid`, `PushToHuawei`)
5. **status/** + **storage/** track success/failure counts across configurable backends

### Key Packages

- **app/**: Application orchestration — CLI send helpers (`sender.go`), config validation/merge (`config.go`), CLI options (`options.go`), queue worker creation (`worker.go`)
- **config/**: Y
```

</details>
