---
name: wesbos__wesbos__skill
source: https://github.com/wesbos/wesbos/blob/38c24a5768536f76be80491ff74951c469cee676/.agent/skills/tip/SKILL.md
repo: wesbos/wesbos
kind: skill
stars: 546
last_pushed: 2026-05-27T20:51:22Z
license: unknown
score: 9
domains: [content-automation, web-development]
tags: [mdx, workflow-automation]
curated: 2026-06-15
curated_by: config-scout
---

# wesbos/wesbos — skill

**Why it's worth keeping:** Demonstrates the 'tool -> fallback tool' pattern for unreliable data fetching and enforces a multi-step workflow including post-action command execution.

**Summary:** Automates converting social media posts into structured MDX content by providing specific CLI commands, fallback browser strategies, and style guidelines.

**Source credibility:** High; Wes Bos is a prominent developer with a well-maintained repository.

**Recency:** Current; reflects modern agent workflows using MCP and CLI tools.

**Source:** [wesbos/wesbos/.agent/skills/tip/SKILL.md](https://github.com/wesbos/wesbos/blob/38c24a5768536f76be80491ff74951c469cee676/.agent/skills/tip/SKILL.md) · 546★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: tip
description: Create a new Hot Tip for wesbos.com
---

# tip

## When to use

When the user asks to create a new tip or edit an existing one. Tips are short-form Hot Tips originally posted to social media (X/Twitter, LinkedIn, TikTok, Instagram, Threads, Bluesky, YouTube Shorts, Reddit, Facebook). The input may be as little as a single social media link.

## Creating a new tip

### 1. Gather the content

- The user will provide the tip text and/or a link to a social media post. They may also accompany a description and/or some code samples.
- **Use `fetchSocial.ts`** to pull post data from a social media URL. It reuses the project's fetchers (`src/lib/socials/`) without needing the app's DB or Cloudflare worker. Run it with:
  ```
  pnpm fetch-social <url>
  ```
  It outputs JSON to stdout (status messages go to stderr). Supports: tiktok, twitter (needs `X_BEARER_TOKEN` env var), linkedin, instagram, bluesky. Key fields vary by platform — look for `desc`/`full_text`/`headline` for the post text and `createTime`/`createdAt`/`datePublished` for the date.
- **Use `listPosts.ts`** to list recent posts or search by keyword. Run it with:
  ```
  pnpm list-posts [twitter|blue
```

</details>
