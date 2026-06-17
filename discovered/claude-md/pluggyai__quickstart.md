---
name: pluggyai__quickstart
source: https://github.com/pluggyai/quickstart/blob/7974a9557f220fb242452bf8e2626a5749f7fc70/CLAUDE.md
repo: pluggyai/quickstart
kind: claude-md
stars: 62
last_pushed: 2026-06-08T22:35:50Z
license: unknown
score: 9
domains: [monorepo, api-integration, web-frontend, backend]
tags: [monorepo-navigation, command-mapping, context-aware-patterns]
curated: 2026-06-14
curated_by: config-scout
---

# pluggyai/quickstart — claude-md

**Why it's worth keeping:** The 'Notable Patterns' section is excellent for warning Claude about deprecated tech/versions, and the command table solves the polyglot execution problem inherent in monorepos.

**Summary:** Provides critical structural navigation and command mapping for a complex, multi-language monorepo. It embeds essential domain knowledge regarding the security model required across all examples.

**Source credibility:** Official documentation from a specialized financial data API provider.

**Recency:** Highly relevant; it explicitly addresses modern vs legacy architectural shifts (e.g., Next.js App Router).

**Source:** [pluggyai/quickstart/CLAUDE.md](https://github.com/pluggyai/quickstart/blob/7974a9557f220fb242452bf8e2626a5749f7fc70/CLAUDE.md) · 62★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

Official Pluggy quickstart repository with integration examples for the Pluggy financial data aggregation API and Connect widget. Complements [Pluggy docs](https://docs.pluggy.ai). Each subdirectory is an independent project with its own dependencies.

## Architecture

```
quickstart/
├── frontend/                    # Client-side integration examples
│   ├── react/                   # React (CRA) + react-pluggy-connect
│   ├── nextjs/                  # Next.js 15 (Pages Router) + pluggy-sdk server-side
│   ├── react-native/            # React Native 0.66 (bare workflow)
│   ├── react-native-expo/       # Expo SDK 54 + expo-router
│   ├── flutter/                 # Flutter WebView integration
│   ├── cordova/                 # Apache Cordova iOS
│   ├── html/                    # Vanilla HTML + CDN script
│   └── flask/                   # Python Flask with templates
├── examples/                    # Backend/deployment examples
│   ├── vercel-quickdeploy-nextjs/  # Full-stack Next.js 16 + Supabase + webhooks
│   ├── node-nestjs/
```

</details>
