---
name: realmorrisliu__sealbox
source: https://github.com/realmorrisliu/sealbox/blob/0408b98df654446e7e5404684345bd9fbd57e497/CLAUDE.md
repo: realmorrisliu/sealbox
kind: claude-md
stars: 5
last_pushed: 2026-06-08T09:37:45Z
license: apache-2.0
score: 9
domains: [backend-api, cli-tools, security, rust]
tags: [rust, encryption, fullstack, api-specification]
curated: 2026-06-15
curated_by: config-scout
---

# realmorrisliu/sealbox — claude-md

**Why it's worth keeping:** The explicit breakdown of the security model (envelope encryption) prevents AI errors in data handling, while the categorized dependency lists provide instant ecosystem awareness.

**Summary:** This file provides deep architectural, security, and operational context for a Rust-based secret management service. It covers the full stack including CLI commands, server API endpoints, and specific encryption logic.

**Source credibility:** High; a well-organized, active Rust project with clear architectural intent.

**Recency:** Very recent; includes modern tech like React 19 and TanStack.

**Source:** [realmorrisliu/sealbox/CLAUDE.md](https://github.com/realmorrisliu/sealbox/blob/0408b98df654446e7e5404684345bd9fbd57e497/CLAUDE.md) · 5★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Sealbox is a lightweight, single-node secret storage service built in Rust. It provides envelope encryption with end-to-end encryption (E2EE) using RSA key pairs, stores data in SQLite, and exposes a REST API for secret management.

### Key Architecture Components

- **sealbox-server/**: Main server application with REST API
  - `api/`: HTTP handlers and routing (Axum framework)
  - `crypto/`: Encryption/decryption logic (RSA + AES-GCM envelope encryption)
  - `repo/`: Data persistence layer (SQLite with rusqlite)
  - `config.rs`: Environment-based configuration
  - `error.rs`: Centralized error handling

- **sealbox-cli/**: Command-line interface for key management and secret operations
  - `commands/`: Command handlers (config, key, secret management)
  - `config.rs`: TOML-based configuration management with environment overrides
  - `output.rs`: Multi-format output support (JSON, YAML, Table)
  - **Note**: CLI reuses server's crypto modules for consistency

### Security Model
- **Server-side encryption**: CLI sends plaintext to server, server
```

</details>
