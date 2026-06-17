---
name: TeklemariamA__motoko-the-civic-os--2-__ii-skill
source: https://github.com/TeklemariamA/motoko-the-civic-os--2-/blob/c8688864766a12ee79ab1725c858bfa7e7bbf653/ii-SKILL.md
repo: TeklemariamA/motoko-the-civic-os--2-
kind: skill
stars: 0
last_pushed: 2026-05-08T01:26:20Z
license: unknown
score: 9
domains: [web-frontend, security, blockchain]
tags: [icp, auth, internet-identity, javascript]
curated: 2026-06-14
curated_by: config-scout
---

# TeklemariamA/motoko-the-civic-os--2- — skill

**Why it's worth keeping:** The 'Mistakes That Break Your Build' section provides critical security and environment-specific troubleshooting logic that prevents common developer errors like using unsafe root key methods.

**Summary:** A highly specialized guide for integrating Internet Identity authentication into ICP frontend applications.

**Source credibility:** Low social proof/stars, but the extreme technical specificity regarding canister IDs and protocol quirks indicates high-quality domain expertise.

**Recency:** Very current, referencing Node.js 22 and modern SDK patterns.

**Source:** [TeklemariamA/motoko-the-civic-os--2-/ii-SKILL.md](https://github.com/TeklemariamA/motoko-the-civic-os--2-/blob/c8688864766a12ee79ab1725c858bfa7e7bbf653/ii-SKILL.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: internet-identity
description: "Integrate Internet Identity authentication. Covers passkey and OpenID login flows, delegation handling, and principal-per-app isolation. Use when adding login, sign-in, auth, passkeys, or Internet Identity to a frontend or canister. Do NOT use for wallet integration or ICRC signer flows — use wallet-integration instead."
license: Apache-2.0
compatibility: "icp-cli >= 0.2.2, Node.js >= 22"
metadata:
  title: Internet Identity Auth
  category: Auth
---

# Internet Identity Authentication

## What This Is

Internet Identity (II) is the Internet Computer's native authentication system. Users authenticate into II-powered apps either with passkeys stored in their devices or thorugh OpenID accounts (e.g., Google, Apple, Microsoft) -- no login or passwords required. Each user gets a unique principal per app, preventing cross-app tracking.

## Prerequisites

- `@icp-sdk/auth` (>= 5.0.0), `@icp-sdk/core` (>= 5.0.0)

## Canister IDs

| Canister | ID | URL | Purpose |
|----------|------------|-----|---------|
| Internet Identity (backend) | `rdmx6-jaaaa-aaaaa-aaadq-cai` |  | Manages user keys and authentication logic |
| Internet Identity (frontend) |
```

</details>
