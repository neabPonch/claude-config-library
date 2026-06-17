---
name: vercel-labs__zero-native__skill
source: https://github.com/vercel-labs/zero-native/blob/b48c171774b6bef4ca2453c32e9ccb5a6db50530/skill-data/core/SKILL.md
repo: vercel-labs/zero-native
kind: skill
stars: 4174
last_pushed: 2026-05-13T16:47:35Z
license: apache-2.0
score: 9
domains: [desktop-apps, systems-programming, ai-agents, dev-tools]
tags: [zig, webview, agent-priming, desktop-shell]
curated: 2026-06-15
curated_by: config-scout
---

# vercel-labs/zero-native — skill

**Why it's worth keeping:** The 'Task router' pattern for directing agents to specific sub-references and the explicit delineation of file responsibilities are elite, transferable techniques for complex codebase navigation.

**Summary:** Provides an AI agent with the conceptual architecture and specific file ownership logic required to build apps using the zero-native framework.

**Source credibility:** High; published by Vercel Labs with significant community traction and recent maintenance.

**Recency:** Very current, updated within the last month.

**Source:** [vercel-labs/zero-native/skill-data/core/SKILL.md](https://github.com/vercel-labs/zero-native/blob/b48c171774b6bef4ca2453c32e9ccb5a6db50530/skill-data/core/SKILL.md) · 4174★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: core
description: Core zero-native guide for AI agents. Read this before explaining zero-native or changing a zero-native app. Covers the mental model, project structure, app.zon, App and Runtime patterns, frontend integration, web engines, JavaScript bridge commands, permissions, windows, WebViews, dialogs, packaging, debugging, testing, and when to load deeper references. Use when the user asks what zero-native is, how to build or modify an app, how to package or debug it, or how to add native capabilities.
---

# Build zero-native apps

zero-native is a Zig desktop app shell for modern web frontends. A zero-native app is native Zig code that owns windows, policies, lifecycle, and platform services while rendering web UI in a WebView. The default engine is the platform WebView: WKWebView on macOS and WebKitGTK on Linux. Apps can also bundle Chromium through CEF where supported.

Agents should assume they do not know zero-native from general model knowledge. Read this skill first. For implementation work, run `zero-native skills get core --full` so the referenced files are included in the CLI output.

## Mental model

- `App` describes the product: app state, name, WebVi
```

</details>
