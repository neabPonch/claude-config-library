---
name: tunnels-is__tunnels__claude
source: https://github.com/tunnels-is/tunnels/blob/781192cbfa2299bbf9d99a3de474eda54f685d12/server/CLAUDE.md
repo: tunnels-is/tunnels
kind: claude-md
stars: 51
last_pushed: 2026-06-11T12:15:36Z
license: other
score: 9
domains: [backend, networking, security, go]
tags: [architecture-map, systems-programming, vpn]
curated: 2026-06-16
curated_by: config-scout
---

# tunnels-is/tunnels — claude-md

**Why it's worth keeping:** Exceptional use of file-to-component mapping with specific line references; detail on configuration-driven feature flags allows the AI to understand how runtime behavior changes.

**Summary:** Provides a comprehensive architectural map of a Go-based VPN server, linking specific files to their functional roles in networking, security, and API management.

**Source credibility:** High quality; active repository with 51 stars and recent maintenance.

**Recency:** Highly current; follows modern best practices for codebase grounding in LLM tool-use workflows.

**Source:** [tunnels-is/tunnels/server/CLAUDE.md](https://github.com/tunnels-is/tunnels/blob/781192cbfa2299bbf9d99a3de474eda54f685d12/server/CLAUDE.md) · 51★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Tunnels.is VPN Server - Context

## Server Overview
The server component is a comprehensive VPN server written in Go that provides VPN connectivity, user management, device management, and API services. It supports multiple features that can be enabled/disabled via configuration.

## Key Files & Components

### Core Files
- **main.go** (`server/main.go:55`): Main entry point, initializes server components and feature flags
- **handlers.go**: HTTP API request handlers for all v3 endpoints
- **new_api.go**: Newer API implementations and server setup
- **types.go**: Server-specific type definitions and core data structures
- **config.json**: Server configuration file with feature toggles and settings

### Database & Storage
- **dbwrapper.go**: MongoDB database operations and user/device/group management
- **bboltwrapper.go**: BoltDB local database operations (alternative to MongoDB)
- **secret_store.go**: Handles secret storage (config file vs environment variables)

### Network & Socket Management
- **socket.go**: Raw socket programming, client connection management, packet handling
- **dhcp.go**: DHCP-style IP assignment for LAN clients
- **ping.go**: Client ping/keepalive functio
```

</details>
