---
name: openai__plugins__skill
source: https://github.com/openai/plugins/blob/c6ea566d43f71cb85ae39a6f7c0c50e287794652/plugins/stripe/skills/upgrade-stripe/SKILL.md
repo: openai/plugins
kind: skill
stars: 3061
last_pushed: 2026-06-11T08:46:18Z
license: unknown
score: 8
domains: [backend-api, fintech]
tags: [stripe, api-migration, sdk]
curated: 2026-06-15
curated_by: config-scout
---

# openai/plugins — skill

**Why it's worth keeping:** It offers highly specific version strings, a clear checklist for manual verification, and 'Good vs Avoid' code examples that prevent common integration errors.

**Summary:** Provides technical constraints and explicit coding patterns required to safely upgrade Stripe API versions across various SDKs.

**Source credibility:** High-quality specialized documentation resembling official Stripe technical guides.

**Recency:** Extremely current/future-dated (2026), making it highly relevant for modern API versioning logic.

**Source:** [openai/plugins/plugins/stripe/skills/upgrade-stripe/SKILL.md](https://github.com/openai/plugins/blob/c6ea566d43f71cb85ae39a6f7c0c50e287794652/plugins/stripe/skills/upgrade-stripe/SKILL.md) · 3061★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: upgrade-stripe
description: Guide for upgrading Stripe API versions and SDKs
---

The latest Stripe API version is 2026-02-25.clover - use this version when upgrading unless the user specifies a different target version.

# Upgrading Stripe Versions

This guide covers upgrading Stripe API versions, server-side SDKs, Stripe.js, and mobile SDKs.

## Understanding Stripe API Versioning

Stripe uses date-based API versions (e.g., `2026-02-25.clover`, `2025-08-27.basil`, `2024-12-18.acacia`). Your account's API version determines request/response behavior.

### Types of Changes

**Backward-Compatible Changes** (do not require code updates):
- New API resources
- New optional request parameters
- New properties in existing responses
- Changes to opaque string lengths (e.g., object IDs)
- New webhook event types

**Breaking Changes** (require code updates):
- Field renames or removals
- Behavioral modifications
- Removed endpoints or parameters

Review the [API Changelog](https://docs.stripe.com/changelog.md) for all changes between versions.

## Server-Side SDK Versioning

See [SDK Version Management](https://docs.stripe.com/sdks/set-version.md) for details.

### Dynamically-Ty
```

</details>
