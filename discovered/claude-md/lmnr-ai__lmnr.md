---
name: lmnr-ai__lmnr
source: https://github.com/lmnr-ai/lmnr/blob/0e1fa422008269f6c4a90ad6441c6bfaa2a1094b/CLAUDE.md
repo: lmnr-ai/lmnr
kind: claude-md
stars: 3002
last_pushed: 2026-06-15T01:07:46Z
license: apache-2.0
score: 9
domains: [backend-api, devops, database-management, fullstack]
tags: [monorepo, architecture, migration-guide]
curated: 2026-06-15
curated_by: config-scout
---

# lmnr-ai/lmnr — claude-md

**Why it's worth keeping:** Includes crucial 'gotcha' instructions for manual database migrations and maintains synchronization rules between frontend/backend schemas to prevent logic errors.

**Summary:** Detailed multi-service monorepo guide covering service dependencies, architecture topology, and specific development workflows.

**Source credibility:** High; from a high-star, YC-backed observability platform repository.

**Recency:** Modern; uses current tooling like uv, pnpm, and Turbopack.

**Source:** [lmnr-ai/lmnr/CLAUDE.md](https://github.com/lmnr-ai/lmnr/blob/0e1fa422008269f6c4a90ad6441c6bfaa2a1094b/CLAUDE.md) · 3002★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Laminar is an open-source observability platform for AI agents. It provides OpenTelemetry-native tracing, evaluations, AI monitoring, and SQL access to all data.

## Repository Structure

This is a multi-service monorepo with three main components:

- **app-server/** - Rust backend (Actix-web HTTP, Tonic gRPC)
- **frontend/** - Next.js/TypeScript web UI
- **query-engine/** - Python gRPC service for SQL query processing
- **pii-redactor/** - optional Rust gRPC service that runs a HuggingFace token-classification PII model on CPU via ONNX Runtime. Standalone — not linked from app-server. Tested with the OpenAI privacy filter (BIOES) and Piiranha (BIO); accepts either scheme via `config.json` `id2label`. See `pii-redactor/README.md` for the gRPC contract, model layout (`model.onnx` + optional `model.onnx_data*` external-data shards + `tokenizer.json` + `config.json`), and the weight-baking Dockerfile.

## Development Commands

### Frontend (Next.js)

```bash
cd frontend
pnpm install                    # Install dependencies
pnpm run dev
```

</details>
