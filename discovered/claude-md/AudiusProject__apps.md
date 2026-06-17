---
name: AudiusProject__apps
source: https://github.com/AudiusProject/apps/blob/5ec7686838732df9f165f3f1523a500430a1fe68/CLAUDE.md
repo: AudiusProject/apps
kind: claude-md
stars: 611
last_pushed: 2026-06-11T21:54:41Z
license: apache-2.0
score: 9
domains: [web, mobile, blockchain, monorepo]
tags: [monorepo, protocol, full-stack, domain-specific]
curated: 2026-06-15
curated_by: config-scout
---

# AudiusProject/apps — claude-md

**Why it's worth keeping:** The 'Terminology' section prevents AI hallucinations regarding deprecated architecture, and the package descriptions provide critical context for navigating a complex monorepo.

**Summary:** This config provides deep domain terminology, a clear breakdown of the monorepo structure, and specific operational commands for local development.

**Source credibility:** High; part of an active open-source project (Audius) with high star count and recent activity.

**Recency:** Current; the repository shows very recent commits.

**Source:** [AudiusProject/apps/CLAUDE.md](https://github.com/AudiusProject/apps/blob/5ec7686838732df9f165f3f1523a500430a1fe68/CLAUDE.md) · 611★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Terminology

Audius runs on the **Open Audio Protocol**, which uses a single canonical node type: the **Open Audio Validator Node**. The earlier split between *Discovery Nodes* and *Content Nodes* is deprecated — both roles are now served by validator nodes. When writing docs, comments, commit messages, or user-facing strings, use "Open Audio Validator Node" (or just "validator node"). Do not introduce new references to "Discovery Node", "Content Node", "Creator Node", or "Discovery Provider". Directory names like `packages/discovery-provider` and `mediorum` are retained for compatibility but no longer reflect the architecture.

## Project Overview

Audius is a decentralized, community-owned music-sharing protocol. This is a monorepo containing:

- Web and desktop applications (React + Vite)
- Mobile applications (React Native)
- Backend services that together make up the Open Audio Validator Node software (indexer + media storage; see `packages/discovery-provider` and `mediorum` directories — names retained from earlier architecture)
- Blockchain smart contracts
```

</details>
