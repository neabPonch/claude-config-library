---
name: Baieti-de-oras-UCluj-Hackathon__ucluj-hackathon
source: https://github.com/Baieti-de-oras-UCluj-Hackathon/ucluj-hackathon/blob/0ad7ee53ad1f6903f85fdb02e5d2112f93e80509/CLAUDE.md
repo: Baieti-de-oras-UCluj-Hackathon/ucluj-hackathon
kind: claude-md
stars: 0
last_pushed: 2026-05-08T07:50:17Z
license: mit
score: 9
domains: [fullstack, machine-learning, mobile-app, design-systems]
tags: [negative-constraints, architecture, design-tokens, auth-flows]
curated: 2026-06-16
curated_by: config-scout
---

# Baieti-de-oras-UCluj-Hackathon/ucluj-hackathon — claude-md

**Why it's worth keeping:** Uses powerful 'negative constraints' to prevent AI scope creep (e.g., 'Never invent or add...', 'Zero border radius') and identifies non-negotiable source files for context alignment.

**Summary:** Provides strict architectural rules, specific command sets for dual-auth environments, and rigid ML feature boundaries. It acts as both a technical manual and a product identity manifesto.

**Source credibility:** Hackathon project; low social proof but demonstrates high-quality documentation standards.

**Recency:** Highly current, updated within the last month.

**Source:** [Baieti-de-oras-UCluj-Hackathon/ucluj-hackathon/CLAUDE.md](https://github.com/Baieti-de-oras-UCluj-Hackathon/ucluj-hackathon/blob/0ad7ee53ad1f6903f85fdb02e5d2112f93e80509/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Is

**UmbraRo** — an AI tactical intelligence assistant for professional Romanian Superliga football coaches. The product operationalises an academic thesis: CatBoost win-probability prediction + constrained Monte Carlo optimisation for prescriptive tactical recommendations.

Before implementing anything, consult **`/AGENTS.md`** (product bible) and **`/design/backend-contract.md`** (supported feature scope). These are non-negotiable constraints, not suggestions.

## Architecture

Two-part system:

**Flutter frontend** (`lib/`) — mobile/web app. Feature-first structure under `lib/features/`; shared infrastructure in `lib/core/`. State management: `ChangeNotifier` + Repository pattern (no Riverpod/Bloc). Runtime API URL loaded from `/config.json` on web. Can run in legacy JWT mode or Firebase Auth mode (controlled by `USE_FIREBASE_AUTH` dart-define).

**FastAPI backend** (`backend/`) — async Python 3.11+. Layered: `api/v1/endpoints/` → `services/` → `data/` loaders. ML bundle (`ml/umbraro_catboost_bundle.joblib`) loaded once at startup via lifespan hook.
```

</details>
