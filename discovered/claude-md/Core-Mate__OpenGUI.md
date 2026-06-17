---
name: Core-Mate__OpenGUI
source: https://github.com/Core-Mate/OpenGUI/blob/7cf28b90866459e74300869766896f953761dd60/CLAUDE.md
repo: Core-Mate/OpenGUI
kind: claude-md
stars: 151
last_pushed: 2026-06-11T15:34:03Z
license: other
score: 9
domains: [agents-ai, mobile-android, backend-api, system-architecture]
tags: [architecture-driven, risk-aware, boundary-enforcement]
curated: 2026-06-15
curated_by: config-scout
---

# Core-Mate/OpenGUI — claude-md

**Why it's worth keeping:** The 'Sensitive Areas' and 'Open-Source Boundaries' sections are exceptional; they teach the AI exactly where it can break things and what intentionally missing features look like, preventing futile attempts to restore private code.

**Summary:** Provides deep architectural context and strictly defines the boundaries between this public release and its private predecessor to prevent hallucinated logic. It identifies high-risk 'crown jewel' modules and handles stub management explicitly.

**Source credibility:** Highly credible; represents a sophisticated, large-scale project with clear distinctions between production and public versions.

**Recency:** Very current; utilizes advanced context-setting techniques highly effective for modern AI coding agents.

**Source:** [Core-Mate/OpenGUI/CLAUDE.md](https://github.com/Core-Mate/OpenGUI/blob/7cf28b90866459e74300869766896f953761dd60/CLAUDE.md) · 151★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# OpenGUI Release - Repository Guide for Claude Code / Codex

## 1. Repository Positioning

This repository is the source-available public release of OpenGUI.

- `server/` comes from the original `coremate` backend and is now the public NestJS service
- `client/` comes from the original `haomai` Android app and is now the public mobile client
- `docs/` contains public-facing architecture and evaluation materials

In the maintainer workspace there may also be sibling directories such as `../coremate` and `../haomai_v0.0.1`. Treat them as reference-only source snapshots. Unless the user explicitly asks otherwise, all public changes should land in **this** repository only.

## 2. Default Working Rules

- Reply to the user in Chinese.
- Use UTF-8 when creating or editing files.
- Treat this repository as the source of truth for current behavior. If README/comments conflict with code, trust code first and then fix docs.
- Keep every change public-release-safe. Never reintroduce private endpoints, production IPs, commercial SDKs, hardcoded credentials, internal dashboards, or company-only workflows.
- Do not edit generated or dependency directories such as `server/node_modules`, `server/
```

</details>
