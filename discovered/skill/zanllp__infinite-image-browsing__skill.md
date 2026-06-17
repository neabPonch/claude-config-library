---
name: zanllp__infinite-image-browsing__skill
source: https://github.com/zanllp/infinite-image-browsing/blob/e1162ab98753cda1d70ec225a03e24b97065243a/skills/iib/SKILL.md
repo: zanllp/infinite-image-browsing
kind: skill
stars: 1315
last_pushed: 2026-06-09T12:49:30Z
license: mit
score: 9
domains: [api-integration, cli-tools, image-management]
tags: [api, automation, local-service]
curated: 2026-06-15
curated_by: config-scout
---

# zanllp/infinite-image-browsing — skill

**Why it's worth keeping:** Includes essential pre-flight connectivity checks, handles proxy/localhost nuances, and defines multi-step asynchronous workflows (start -> status -> confirm) alongside specific UI presentation logic.

**Summary:** A comprehensive skill file that enables an agent to manage a local image service via API, covering search, organization, and metadata extraction.

**Source credibility:** High; source repository is a popular, actively maintained image management tool.

**Recency:** Very current; specifically optimized for agentic interaction via curl and local service discovery.

**Source:** [zanllp/infinite-image-browsing/skills/iib/SKILL.md](https://github.com/zanllp/infinite-image-browsing/blob/e1162ab98753cda1d70ec225a03e24b97065243a/skills/iib/SKILL.md) · 1315★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: iib
description: Interact with IIB (Infinite Image Browsing) service for searching, browsing, tagging, and organizing AI-generated images. Use when the user needs to search images by prompt/keyword, manage image tags, organize files into folders, get image generation parameters, or work with an image library.
---

# IIB (Infinite Image Browsing)

IIB is an image/video browsing and management tool that parses metadata from AI generation tools (Stable Diffusion, ComfyUI, etc.).

---

## Quick Links to Detailed Guides

| Topic | Description |
|-------|-------------|
| **[API Reference](references/api-reference.md)** | Complete API endpoint documentation |
| **[Search Strategies](references/search-strategies.md)** | Multi-word, regex, tag combination searches |
| **[Agent Patterns](references/agent-patterns.md)** | Common workflows and decision trees |

---

## Before You Start

**IMPORTANT:** Always do these two things first:

1. **Ask the user for the port** if they started the service themselves (common ports: `<port>` standalone, `7860` SD WebUI extension)
2. **Test connectivity** with a hello request before any other operation

```bash
curl --noproxy "*" -s http://127.0.
```

</details>
