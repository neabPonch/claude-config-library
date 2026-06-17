---
name: grace-xwerks__use-chat
source: https://github.com/grace-xwerks/use-chat/blob/92413b4896056092c3d9082c3d0bd3e01e77e9cb/claude.md
repo: grace-xwerks/use-chat
kind: claude-md
stars: 0
last_pushed: 2026-06-01T18:02:10Z
license: unknown
score: 7
domains: [web-extension, javascript]
tags: [chrome-extension, implementation-intent]
curated: 2026-06-14
curated_by: config-scout
---

# grace-xwerks/use-chat — claude-md

**Why it's worth keeping:** Uses 'Current behavior' to document implementation nuances (like debouncing/polling) that prevent regressions and includes a 'Planned v2' section to guide AI-assisted development.

**Summary:** Provides highly specific context for a Chrome extension, including business logic and delicate DOM manipulation strategies.

**Source credibility:** Low; appears to be an internal organizational tool with no public social proof.

**Recency:** 

**Source:** [grace-xwerks/use-chat/claude.md](https://github.com/grace-xwerks/use-chat/blob/92413b4896056092c3d9082c3d0bd3e01e77e9cb/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
\# use-chat — Chrome Extension



Internal Chrome extension for Grace Engineering (grace-xwerks).

Detects internal @graceeng.com recipients in Gmail compose windows

and nudges the sender to use Google Chat instead.



\## Org context

\- Domain: graceeng.com

\- Chat URL: https://chat.google.com

\- Deployed via: Chrome managed extensions (Workspace admin)

\- Repo: grace-xwerks/use-chat



\## Extension structure

\- manifest.json   — MV3 manifest

\- content.js      — Content script, injected into mail.google.com

\- styles.css      — Banner styles injected alongside content.js



\## Current behavior (v1)

\- MutationObserver watches for Gmail compose windows (popup + full-screen)

\- Polling fallback (250ms × 20, then 3s) catches already-open windows

\- Debounced observer (150ms) prevents infinite loop on DOM mutation

\- Detects internal recipients via data-hovercard-id and span\[email] attributes

\- Injects a dismissable banner above the message body when internal

&#x20; recipients are present

\- Banner has "Open Chat" link and a dismiss button



\## Planned v2 features

1\. Deep link DM button — link to chat.google.com/dm/\[email]

2\. Show recipient display names in
```

</details>
