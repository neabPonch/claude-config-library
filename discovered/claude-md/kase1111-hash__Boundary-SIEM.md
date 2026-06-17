---
name: kase1111-hash__Boundary-SIEM
source: https://github.com/kase1111-hash/Boundary-SIEM/blob/f7f34c2c0bae67c147feb8add5c4e7a5123f5c5c/claude.md
repo: kase1111-hash/Boundary-SIEM
kind: claude-md
stars: 2
last_pushed: 2026-04-08T02:57:15Z
license: mit
score: 9
domains: [backend, security, cli-tools, go]
tags: [go, siem, architecture-heavy, workflow-driven]
curated: 2026-06-15
curated_by: config-scout
---

# kase1111-hash/Boundary-SIEM — claude-md

**Why it's worth keeping:** The 'Common Tasks' section is excellent for LLMs as it provides procedural knowledge for system expansion, while the ASCII architecture map gives immediate context of data flow.

**Summary:** Provides a high-density technical roadmap including architecture diagrams, specific development workflows, and strict coding standards.

**Source credibility:** Low star count, but the documentation depth suggests a highly engineered, professional-grade project.

**Recency:** Current; uses modern Go 1.24 and contemporary toolchain patterns.

**Source:** [kase1111-hash/Boundary-SIEM/claude.md](https://github.com/kase1111-hash/Boundary-SIEM/blob/f7f34c2c0bae67c147feb8add5c4e7a5123f5c5c/claude.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Boundary-SIEM

Blockchain-native Security Information and Event Management (SIEM) platform designed for decentralized infrastructure, validator networks, and AI agent ecosystems.

## Tech Stack

- **Language**: Go 1.24.7
- **Database**: ClickHouse (time-series analytics)
- **Message Queue**: Kafka
- **Session Store**: Redis
- **TUI Framework**: Charmbracelet (Bubbletea + Lipgloss)
- **Encryption**: AES-256-GCM
- **Parsing**: CEF, JSON, Syslog

## Architecture Overview

```
┌─────────────────────────────────────────────────────┐
│              USER INTERFACES                         │
│  ├─ Terminal UI (TUI) - Dashboard & Event Browser  │
│  ├─ REST API (/api/v1/*)                            │
│  ├─ GraphQL (/graphql)                              │
│  └─ WebSocket (Real-time alerts)                    │
├─────────────────────────────────────────────────────┤
│          APPLICATION TIER (INGEST SERVICE)           │
│  ├─ CEF Parser (UDP 5514/TCP 5515/DTLS 5516)       │
│  ├─ JSON HTTP Ingestion                              │
│  ├─ Event Normalization & Schema Validation         │
│  ├─ Correlation Engine                               │
│  ├─ Detection Engine (143 blockchain rules)
```

</details>
