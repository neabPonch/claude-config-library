---
name: Caldis__react-zmage
source: https://github.com/Caldis/react-zmage/blob/bd9b97db87a969ebf64306f6f944ea2ff4bbbd2a/SKILL.md
repo: Caldis/react-zmage
kind: skill
stars: 936
last_pushed: 2026-05-18T17:26:31Z
license: mit
score: 9
domains: [web-frontend, react]
tags: [image-viewer, integration-pattern, documentation-driven]
curated: 2026-06-14
curated_by: config-scout
---

# Caldis/react-zmage — skill

**Why it's worth keeping:** The 'Read first' pattern of fetching llms.txt is a top-tier technique for keeping agents updated; additionally, it provides clear decision logic between Component, Wrapper, and Imperative modes.

**Summary:** This skill provides specific implementation patterns for integrating the react-zmage image viewer into various React environments. It includes a critical directive to fetch external documentation first to ensure accuracy.

**Source credibility:** Strong; the repository has high star count (936) and recent activity.

**Recency:** Highly current; utilizes modern agentic documentation patterns like llms.txt.

**Source:** [Caldis/react-zmage/SKILL.md](https://github.com/Caldis/react-zmage/blob/bd9b97db87a969ebf64306f6f944ea2ff4bbbd2a/SKILL.md) · 936★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: react-zmage-integration
description: Use when adding the react-zmage React image viewer to an existing React, Next.js, MDX, CMS, markdown, or rich text image surface.
---

# react-zmage Integration

## When to use this skill

Use this skill when a user wants fullscreen image preview, image zoom, a React lightbox alternative, CMS image preview, MDX image preview, or gallery browsing in a React app.

Do not use this skill for unrelated image processing, server-side media transformation, account automation, OAuth setup, webhook setup, or MCP server work. react-zmage is a client-side React package.

## Read first

Fetch https://zmage.caldis.me/llms.txt first. Use https://zmage.caldis.me/llms-full.txt when you need the full README and repository agent notes in one request.

Install with:

```bash
npm install react-zmage
```

Import the stylesheet once from the app-level style entry:

```ts
import 'react-zmage/style.css'
```

Choose the smallest mode that matches the user's image surface:

- Component mode for owned React image markup: `<Zmage src="..." alt="..." />`.
- Wrapper mode for CMS, MDX, markdown, rich text, or generated HTML: `<Zmage.Wrapper>{children}</Zmage.Wrapper>
```

</details>
