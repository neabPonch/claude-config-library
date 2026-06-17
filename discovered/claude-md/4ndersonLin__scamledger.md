---
name: 4ndersonLin__scamledger
source: https://github.com/4ndersonLin/scamledger/blob/45d36e8a08af00a9330babc37c848c6b4aaa6cf8/claude.md
repo: 4ndersonLin/scamledger
kind: claude-md
stars: 0
last_pushed: 2026-02-27T16:17:47Z
license: unknown
score: 9
domains: [web-frontend, backend-api, security, crypto]
tags: [monorepo, cloudflare-workers, typescript, fullstack]
curated: 2026-06-14
curated_by: config-scout
---

# 4ndersonLin/scamledger — claude-md

**Why it's worth keeping:** It includes actionable mathematical formulas (risk score calculation) and clear architectural constraints (dual API layers). The highly granular coding conventions prevent common AI hallucinations in naming and type safety.

**Summary:** Provides a comprehensive blueprint for a full-stack monorepo using the Cloudflare ecosystem. It covers everything from directory structure to specific business logic formulas.

**Source credibility:** Low social proof due to 0 stars, but the technical density suggests a real, sophisticated project.

**Recency:** Very current; utilizes modern technologies like React 19 and ESLint v9 flat config.

**Source:** [4ndersonLin/scamledger/claude.md](https://github.com/4ndersonLin/scamledger/blob/45d36e8a08af00a9330babc37c848c6b4aaa6cf8/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — CryptoScamReport

## Project Overview

CryptoScamReport is a free, community-powered cryptocurrency scam and hack incident reporting platform. Users can anonymously report scam/hack incidents and search known threat addresses. A Developer API (with Passkey registration + API Key) is available for third-party integrations.

- **Website frontend**: Fully public, no login required
- **Developer API (`/v1/*`)**: Requires API Key (register via Passkey)
- **Design reference**: See `CryptoScamReport-Design-v1.4.md` for full specs

## Tech Stack

| Layer            | Technology                                 |
| ---------------- | ------------------------------------------ |
| Frontend         | React 19 + Vite + TypeScript + TailwindCSS |
| Backend API      | Cloudflare Workers + Hono framework        |
| Database         | Cloudflare D1 (SQLite)                     |
| Cache / Sessions | Cloudflare KV                              |
| Bot protection   | Cloudflare Turnstile                       |
| Auth             | WebAuthn Passkey (`@simplewebauthn`)       |
| i18n             | react-i18next (zh-TW / en)                 |
| Charts           | Recharts
```

</details>
