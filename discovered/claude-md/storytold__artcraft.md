---
name: storytold__artcraft
source: https://github.com/storytold/artcraft/blob/0de867ad13999a8f4f8e7771618f738e4b8e0b73/CLAUDE.md
repo: storytold/artcraft
kind: claude-md
stars: 1684
last_pushed: 2026-06-15T02:20:29Z
license: other
score: 9
domains: [backend-api, desktop-app, monorepo]
tags: [rust, typescript, monorepo, structural-patterns]
curated: 2026-06-15
curated_by: config-scout
---

# storytold/artcraft — claude-md

**Why it's worth keeping:** The highly detailed directory tree explains the relationship between crates, while the 'File Layout' section provides predictable patterns for generating consistent file structures.

**Summary:** Provides an exhaustive architectural map of a complex Rust/TypeScript monorepo and strict guidelines for code structural hierarchy.

**Source credibility:** High; comes from a popular (1.6k+ stars) and actively maintained production-grade repository.

**Recency:** Current; uses modern tooling like SQLx and Actix-web, optimized for contemporary AI coding workflows.

**Source:** [storytold/artcraft/CLAUDE.md](https://github.com/storytold/artcraft/blob/0de867ad13999a8f4f8e7771618f738e4b8e0b73/CLAUDE.md) · 1684★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance for Claude Code when working with the Artcraft monorepo.

## Project Overview

Artcraft is a web and desktop application for generating AI image and video. It is written in 
Rust and TypeScript and contains desktop, server, and frontend components.

## Project Structure

```
artcraft/
├── _database/                           # Schema definitions and migrations (MySQL, SQLite, Elasticsearch, etc.)
│   ├── elasticsearch/                   # Elasticsearch schema and queries
│   └── sql/                             # MySQL and SQLite schema definitions and migrations
│       ├── artcraft_migrations/         # ArtCraft desktop app SQLite migrations
│       ├── migrations/                  # Server MySQL migrations
│       └── migrations_squashed/         # Fully materialized MySQL schema definitions for most tables
├── _tools/                              # Various 3rd party tool integrations and configurations
│   └── postman/                         # Postman configs for test HTTP requests against development and production
├── build/                               # Dockerfile build instructions for server components
├── crates/
```

</details>
