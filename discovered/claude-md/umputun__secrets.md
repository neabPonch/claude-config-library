---
name: umputun__secrets
source: https://github.com/umputun/secrets/blob/9e7db2599b918b337e5d912239f556832017420b/CLAUDE.md
repo: umputun/secrets
kind: claude-md
stars: 194
last_pushed: 2026-06-08T21:14:12Z
license: apache-2.0
score: 9
domains: [backend-api, security, go]
tags: [architecture-heavy, interface-driven, cryptography]
curated: 2026-06-15
curated_by: config-scout
---

# umputun/secrets — claude-md

**Why it's worth keeping:** It includes explicit interface definitions and precise logic rules (like file header validation) that prevent the AI from introducing breaking changes in sensitive crypto paths. The command section is highly actionable for all development stages.

**Summary:** Provides a deep architectural blueprint including specific Go interfaces, data flow requirements, and critical security/validation constraints.

**Source credibility:** Highly credible; popular repository with active maintenance and significant star count.

**Recency:** Very current, utilizing modern Go features like embed and providing context ideal for today's coding agents.

**Source:** [umputun/secrets/CLAUDE.md](https://github.com/umputun/secrets/blob/9e7db2599b918b337e5d912239f556832017420b/CLAUDE.md) · 194★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Safesecret is a Go-based web service for sharing sensitive information securely. It encrypts messages with a PIN, stores them temporarily, and allows one-time retrieval. The service uses SQLite for storage (both in-memory and persistent modes).

**Hybrid Encryption:** Route-based encryption mode where UI (web browser) always uses zero-knowledge client-side encryption (Web Crypto API AES-128-GCM), while API always uses server-side encryption. This provides maximum security for interactive users while maintaining API simplicity.

## Build and Development Commands

### Run the application
```bash
# Build and run locally (single domain)
cd app && go build -o secrets && ./secrets --key=<SIGN_KEY> --domain=localhost --protocol=http

# Build and run locally (multiple domains)
cd app && go build -o secrets && ./secrets --key=<SIGN_KEY> --domain="localhost,127.0.0.1" --protocol=http

# Run with Docker (development)
docker-compose -f docker-compose-dev.yml up
```

### Testing
```bash
# Run all tests
go test -v -timeout=60s -covermode=count -coverprofile=co
```

</details>
